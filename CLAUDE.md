# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This repository contains presentation materials for the **115 年度 AI 推動實務種子人才研習班（第二期）** — a government AI training workshop. The presenter is 邱毓權 (第五組) from 高雄市政府都市發展局 都市設計科.

The presentation topic is: **AI Agent 都市設計審議助理系統** — an AI Agent that autonomously executes the review workflow to reduce manual burden in urban design approval processes.

## Files

| File | Purpose |
|------|---------|
| `slides_115AI研習班個人簡報.html` | Desktop slide deck (10 slides, keyboard/dot navigation) |
| `slides_115AI研習班個人簡報.pdf` | PDF export (9 pages, animation slide excluded) |
| `index.html` | Mobile RWD version (scroll reading, IntersectionObserver animations) |
| `slide_agent_workflow.html` | Standalone animated workflow page (also embedded in desktop slide 4) |
| `workflow_diagram.svg` | Static workflow diagram — vector, 1200×670 |
| `workflow_diagram.png` | Static workflow diagram — raster PNG, 1200×670 |
| `115AI研習班簡報_NotebookLM素材.txt` | Full plain-text version for NotebookLM input |
| `115 年度 AI 推動實務種子人才研習班_個人簡報_Prompt.txt` | Original generation prompt + scoring rubric |
| `大頭貼.jpg` | Presenter's profile photo |

## Presentation Structure

Desktop deck has 10 slides (s0–s9); mobile `index.html` is a single scrollable page with the same sections.

| Slide | ID | Content |
|-------|----|---------|
| 封面 | s0 | Title slide |
| P1 | s1 | 痛點現場 — 7 staff, ~100 cases/year, ~200 person-days/year |
| P2 | s2 | AI Agent 架構 — tool-chain framing (OCR / RAG / LLM / Speech / Diff) |
| P2+ | s_workflow | AI Agent 融入都審工作流程（animated, iframe on desktop / native HTML on mobile） |
| P3 | s3 | 短期可驗證 — 90-day POC, KPIs ≥30% / ≥85% |
| P4 | s4 | 推動承諾 — timeline, budget (城鄉發展基金) |
| 附錄 A–D | s5–s8 | Roadmap / TCO / stats / LINE Bot proof-of-concept |

## PDF Generation

Uses Playwright + ImageMagick. Script at scratchpad `gen_pdf.mjs`, run from the directory where `playwright` is installed (`~/.npm/_npx/5e2e484947874241/`). Captures slides s0–s8 (9 slides; s_workflow excluded via `print: display:none`).

```
node gen_pdf.mjs
```

## Scoring Rubric (for content validation)

The presentation is scored on three dimensions (5 points each):
1. **問題清晰度** — Must quantify: affected staff, steps, time cost
2. **解方可行性** — Must show: specific tools, data inventory, short-term verification plan
3. **推動意願** — Must demonstrate: supervisor support, budget plan, concrete action commitments

When reviewing or updating slide content, verify each slide covers its corresponding scoring anchor points from the rubric in `_Prompt.txt`.

## Key Data Points (do not alter without source confirmation)

- 承辦員額: 7 人
- 年均案量: ~100 件/年；當前在辦: 59 件
- 年耗人工: ~200 人日/年
- 歷史入庫案件: 3,884 件；會議決議: 97,127 條；會議場次: 2,882 場
- POC 目標: 複查工時縮減 ≥ 30%，格式準確率 ≥ 85%
- 預算來源: 高雄市城鄉發展及都市更新基金
