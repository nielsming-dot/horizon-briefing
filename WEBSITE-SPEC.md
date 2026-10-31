# 个人资讯简报网站 · 对接规格文档

> 本文档面向网站开发（AI 辅助开发亦可直接参照执行），说明数据从哪来、什么格式、网站要做什么。

## 1. 系统背景

上游已有一套**自动运行的资讯简报管道**，无需网站侧做任何采集：

- 仓库：`https://github.com/nielsming-dot/horizon-briefing`（public）
- 运行方式：GitHub Actions 每日 UTC 23:00（北京时间早 7 点）自动执行，产出前一天 24 小时内的简报
- 管道流程：45+ 个 RSS/聚合信源抓取 → GLM 按领域打分过滤（0-10 分）→ 高分条目生成深度摘要（背景/影响/参考链接）→ 中英双语 Markdown 简报
- 产出：每天 1 期，中英各一份，一般 40-80 条入选，目前历史从 2026-10-25 起

**12 个领域**（简报中的版块顺序）：

| # | 版块名 | profile ID |
|---|---|---|
| 1 | AI 动态 | ai-news |
| 2 | 科技新闻 | tech-news |
| 3 | 医学前沿 | medicine-news |
| 4 | 物理学 | physics-news |
| 5 | 天文学 | astronomy-news |
| 6 | 航天动态 | aerospace-news |
| 7 | 化工与化学 | chemical-news |
| 8 | 化工品市场 | chem-products |
| 9 | 能源动态 | energy-news |
| 10 | 油气工业 | oil-gas-news |
| 11 | 教育动态 | education-news |
| 12 | 文学动态 | literature-news |

## 2. 数据获取方式（已验证）

### 2.1 主数据源：gh-pages 分支的 Markdown 文件

每日简报最终持久化在仓库 **gh-pages 分支**的 `_posts/` 目录，文件名规则：

```
_posts/YYYY-MM-DD-summary-zh.md   # 中文版
_posts/YYYY-MM-DD-summary-en.md   # 英文版
```

**直读 URL 模式**（无需任何 token，已验证支持 CORS `access-control-allow-origin: *`，支持 ETag 缓存）：

```
https://raw.githubusercontent.com/nielsming-dot/horizon-briefing/gh-pages/_posts/2026-10-31-summary-zh.md
```

**列出全部可用日期**（GitHub API，免 token，60 次/小时/IP 限流足够）：

```
https://api.github.com/repos/nielsming-dot/horizon-briefing/contents/_posts?ref=gh-pages
```

### 2.2 辅助数据源：RSS（适合做「最新一期」的轻量获取）

```
https://nielsming-dot.github.io/horizon-briefing/feed.xml      # 全部（Jekyll feed）
https://nielsming-dot.github.io/horizon-briefing/feed-zh.xml   # 中文
https://nielsming-dot.github.io/horizon-briefing/feed-en.xml   # 英文
```

### 2.3 更新节奏

每天北京时间 **07:00 触发、约 08:00 前后发布完毕**（任务耗时 40-60 分钟）。偶尔 GitHub 定时任务有 1-2 小时延迟，网站取不到「今天」的数据时要优雅降级显示最近一期。

## 3. 简报 Markdown 结构规范（解析契约）

网站的核心工作是解析这个格式。以 2026-10-29 中文版真实内容为例：

### 3.1 文件总体结构

```markdown
---
layout: default
title: "Horizon Summary: 2026-10-29 (ZH)"
date: 2026-10-29
lang: zh
---

> 从 356 条内容中筛选出 76 条重要资讯。        ← 总览行（数字可用）

---

**AI 动态**                                    ← 目录区开始（粗体领域名 + 编号列表）
1. [条目标题](#item-ai-news-1) ⭐️ 8.0/10
2. [条目标题](#item-ai-news-2) ⭐️ 7.0/10

**科技新闻**
1. [条目标题](#item-tech-news-1) ⭐️ 9.0/10

---

## AI 动态                                     ← 正文区开始（## 二级标题 = 领域）

<a id="item-ai-news-1"></a>                   ← 条目锚点（id 规则：item-{profile}-{序号}）
### [条目标题](原文链接) ⭐️ 8.0/10            ← 三级标题：[标题](原文链接) + 分数

摘要正文，一到多个段落……

来源类型 · 来源名 · 10月29日 14:00             ← 来源行（见 3.3）

**「背景」** ……                                ← 可选的标签块（见 3.4）

**「影响」** ……                                ← 可选

<details><summary>参考链接</summary>           ← 可选的参考链接折叠块
<ul>
<li><a href="...">标题</a></li>
</ul>
</details>

**标签**: `#tag1`, `#tag2`, `#tag3`            ← 标签行

---                                            ← 条目分隔线

<a id="item-ai-news-2"></a>
...
```

### 3.2 需要解析出的结构化字段（每条条目）

| 字段 | 提取方式 |
|---|---|
| 领域 profile | 锚点 id 中的 `item-{profile}-{n}`，或所属 `## 版块` |
| 标题 | `### [标题](url)` 的链接文本 |
| 原文链接 | 同上链接 href |
| 分数 | `⭐️ X.0/10` |
| 摘要 | 来源行之前的所有段落 |
| 来源类型/来源名/时间 | 来源行按 `·` 分割（RSS 条目是 `rss · OilPrice.com · 10月28日 16:00`；HN 条目是 `hackernews · 用户名 · 时间 · [社区讨论](链接)`，多一段可选） |
| 背景块/影响块 | `**「标题」**` 开头的粗体标签段落，**标题文字是 AI 生成的、不固定**（如「背景」「政策背景」「影响」「市场影响」「对XX的影响」），按「位置和措辞风格」识别即可：紧跟摘要的叙述性标签块 |
| 参考链接 | `<details><summary>参考链接</summary>` 内的 `<li><a>` 列表 |
| 标签 | `**标签**: `` `#tag` `` , ...` 反引号包裹的 # 开头词 |

### 3.3 已知的解析坑（务必处理）

1. **HTML 实体双重转义**：标题里会出现 `&\#x27;`、`&amp;#x2019;` 这种被转义两次的实体（原文 `&#x27;` 再被转成 `&amp;#x27;`）。解析时需要做一轮反转义修正：把 `&amp;#` 还原成 `&#` 再正常 unescape。
2. **Google News 跳转链接**：部分原文链接是 `news.google.com/rss/articles/...` 的长跳转 URL，不是最终文章页。展示时照常外链即可，不要试图解析。
3. **分数渲染**：`⭐️ 8.0/10` 中的 ⭐️ 是 emoji，自行决定保留或替换成样式化的分数徽章。
4. **中英文件结构一致**，仅语言不同；条目锚点 id 在中英文件中一一对应，可做双语切换时定位同一条目。

## 4. 网站功能需求

### 4.1 页面

1. **首页**：最新一期简报入口（大卡片：日期 + 入选条数 + 各领域条数分布）+ 历史日期列表（倒序，显示每天的条数）
2. **日报页**（核心页面）：
   - 顶部：日期、总览（从 N 条筛选出 M 条）、中/英切换
   - 左侧（桌面）/顶部（移动）：领域导航目录，显示各领域条数
   - 正文：按领域分组的条目卡片流
   - 条目卡片：标题（外链原文 ↗）、分数徽章、领域标签、摘要、背景/影响折叠展示、参考链接折叠、标签 chips、来源与时间
3. **领域页**（可选，二期）：单一领域的跨日期聚合视图
4. **搜索**（二期）：客户端全文检索历史简报（数据量小，几期几十条，前端索引足够）

### 4.2 交互细节

- 所有原文外链 `target="_blank" rel="noopener"`
- 锚点导航与目录联动（点击目录滚动到条目）
- 深色模式跟随系统
- 移动端优先适配（阅读场景大概率在手机）

### 4.3 数据获取与缓存策略（建议）

- 服务端获取 raw.githubusercontent.com（Next.js Route Handler / Server Component / Astro loader 均可）
- 缓存策略：`revalidate` 每小时，或访问时若当天文件 404 则回退最近一期并短缓存
- **不要**在构建时把所有历史拉死——数据每天新增，运行时获取 + 缓存即可

## 5. 授权访问（原始需求，重要）

需求：**网站仅限授权用户访问**。注意数据本身在 GitHub 公开仓库（已确认可接受公开），授权控制只需要做在网站层。两个方案：

| 方案 | 做法 | 适合 |
|---|---|---|
| **A. Cloudflare Access（推荐）** | 网站部署到 Cloudflare Pages（或任意自定义域名套 CF），开启 Zero Trust Access，邮箱 OTP 验证，免费版 50 用户 | 不想写登录逻辑，快速上线 |
| B. 应用层登录 | NextAuth/Auth.js 做简单的邮箱魔法链接或用户名密码，用户量小用配置文件管理账号即可 | 想要完全自控、以后加用户体系 |

推荐 A：零代码、可加多个授权邮箱、和部署平台解耦。

## 6. 技术选型建议

- **框架**：Next.js（App Router）或 Astro——都是 fetch Markdown → 解析 → 渲染的简单形态，不需要数据库
- **Markdown 解析**：`unified`/`remark` 生态，或按第 3 节契约写自定义解析器（结构非常规律，正则 + 状态机 200 行内可完成，且更可控）
- **部署**：Vercel 或 Cloudflare Pages（都免费额度充足）；若选方案 A 授权，Cloudflare 全家桶更顺

## 7. 边界与注意事项

1. **只读**：网站只从 gh-pages 分支读数据，绝不改动 `nielsming-dot/horizon-briefing` 仓库的代码、工作流和配置
2. **容错**：单日文件缺失（任务延迟/失败）时显示最近一期并提示日期；某条目字段缺失（如无背景块）时正常渲染其余部分
3. **版权口径**：简报是 AI 生成的公开资讯摘要，正文含原文链接与来源标注，网站展示时保留来源信息即可
4. **数据规模**：每天 1 期 × 中英 2 文件 × 40-80 条，一年约 3 万条目，无需考虑性能问题

## 8. 未来扩展（网站侧预留，不必现在实现）

- 管道侧可加一步导出**结构化 JSON**（每日一个 JSON 文件放 gh-pages），届时网站解析层可整体简化——当前 Markdown 契约稳定，先按它做
- 周报/月报聚合视图
- 收藏与个人标注（需引入轻量存储，如 KV/数据库）
- 订阅推送（邮件/飞书 Webhook——管道本身已支持 webhook 输出，开配置即可）
