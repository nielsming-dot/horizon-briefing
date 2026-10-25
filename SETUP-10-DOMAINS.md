# 十领域资讯简报配置说明

本仓库基于 [Thysrealm/Horizon](https://github.com/Thysrealm/Horizon) 配置了 10 个领域的每日资讯简报：AI、科技、医学、物理学、天文学、航天、化工、能源、教育、文学。

## 改动清单（相对上游）

| 位置 | 内容 |
|---|---|
| `profiles/` 新增 9 个 | `ai-news`、`medicine-news`、`physics-news`、`astronomy-news`、`aerospace-news`、`chemical-news`、`energy-news`、`education-news`、`literature-news`，每个含 profile.json + match/analysis/enrichment 提示词 |
| `data/config.github.json` | 全量重写：43 个启用 RSS 源 + HN + Reddit r/MachineLearning + GitHub releases（vLLM/SGLang/Triton） |
| `data/config.json` | 同上（本地运行用） |
| `.github/workflows/daily-summary.yml` | 已从 `.disabled` 启用，每日 UTC 23:00（北京 07:00）运行 |
| `src/orchestrator.py` | 抓取客户端加浏览器 UA（量子位、phys.org 拒绝默认 python UA） |
| `.env` | 已创建（gitignore 内），填 API key 后可本地跑 |

## 各领域信源

- **AI 动态**：The Decoder、量子位、HF Blog、Import AI、HF Daily Papers（经 rsshub.rssforever.com）、MIT TR AI、Reddit ML；arXiv cs.AI 已配置但默认关闭（量大、费用高，HF Papers 已覆盖精华）
- **科技新闻**：Hacker News（≥100分）、Ars Technica、The Verge、TechCrunch、少数派
- **医学前沿**：NEJM、Lancet、Nature Medicine、BMJ、STAT、MedPage Today
- **物理学**：Physics World、Quanta、Phys.org Physics、ScienceDaily Physics
- **天文学**：Space.com、Astronomy.com、EarthSky、ScienceDaily Astronomy、Phys.org Space
- **航天动态**：SpaceNews、Spaceflight Now、NASA News Releases、Ars Science
- **化工与化学**：Phys.org Chemistry、ScienceDaily Chemistry、Nature Chemistry（C&EN / Chemistry World 无可用 RSS，候选见下）
- **能源动态**：Canary Media、Carbon Brief、CleanTechnica、ScienceDaily Energy
- **教育动态**：EdSurge、The 74、Hechinger Report（均偏美国视角）
- **文学动态**：Literary Hub、The Millions、Guardian Books、NYT Books

## 验证情况（2026-10-25）

- 全部源经过 curl 三轮筛选 + Horizon 真实抓取器冒烟测试；36 小时窗口取回 169 条，10 个领域全部有产出
- NASA Science News 因源本身 XML 格式错误被移除
- 本机代理（fake-IP DNS）会拦截 trafilatura 全文抓取（198.18.x.x 报错），不影响 GitHub Actions 运行
- `uv run --extra dev pytest tests/test_rss.py` 全部通过

## 启用步骤

1. 在 GitHub 上 fork 本仓库（或推送到自己的仓库，需 public 才能 free 跑 Actions + Pages）
2. 仓库 Settings → Secrets and variables → Actions 添加 `ZHIPU_API_KEY`（默认 provider 为智谱 GLM，走 OpenAI 兼容通道 + `glm-4.7-flash`；换 DeepSeek/OpenAI/Gemini 需同步改 `data/config.github.json` 的 `ai` 段和 workflow 的 env 映射）
3. Settings → Pages → Source 选 `gh-pages` 分支
4. Actions 页手动触发一次 `Daily Horizon Summary` 验证；之后每天 UTC 23:00 自动运行
5. 产物：`data/summaries/horizon-YYYY-MM-DD-{zh,en}.md`（提交回仓库）+ `docs/_posts/`（发布到 Pages 网站）

## 本地运行（不走 GitHub）

```bash
# .env 里填好 ZHIPU_API_KEY 后：
uv run horizon --hours 24
```
简报落在 `data/summaries/`。定时可用 cron / launchd（macOS）。注意：本机代理若使用 fake-IP DNS，trafilatura 全文抓取会被 SSRF 防护拦截（198.18.x.x 报错），需将相关资讯域名设为直连，或接受仅用 RSS 自带摘要。

## 后续可加的信源（当时不可用）

- 化工：C&EN、Chemistry World（无 RSS / Cloudflare 拦截）→ 可自建 RSSHub 实例补
- 教育：芥末堆（RSSHub 公共实例路由失效）
- 中文科技：36氪（feed 返回非 XML）、机器之心（同）
- 天文：Sky & Telescope（Cloudflare 拦截）
