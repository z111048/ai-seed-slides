# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This repository contains presentation materials for the **115 年度 AI 推動實務種子人才研習班（第二期）** — a government AI training workshop. The presenter is 邱毓權 (第五組) from 高雄市政府都市發展局 都市設計科.

The presentation topic is: **AI 輔助都市設計審議報告書檢核系統** — an AI-assisted system to reduce manual review burden in urban design approval workflows.

## Files

| File | Purpose |
|------|---------|
| `115 年度 AI 推動實務種子人才研習班_個人簡報_Prompt.txt` | Original prompt used to generate the slide content, including the scoring rubric and brief structure |
| `115AI研習班簡報_NotebookLM素材.txt` | Full plain-text version of the 5-slide presentation + appendix, intended as NotebookLM input. Contains all quantitative data, timeline, budget estimates, and design prompt for each slide. |
| `slides_115AI研習班個人簡報.html` | Rendered HTML presentation (the deliverable) |
| `slides_115AI研習班個人簡報.pdf` | PDF export of the presentation |
| `大頭貼.jpg` | Presenter's profile photo |

## Presentation Structure

- **封面**: Title slide
- **P1 — 痛點現場**: Problem scope — 7 staff, ~100 cases/year, ~200 person-days/year lost to format review
- **P2 — AI 解方**: 5-technology stack (LLM, OCR, Vision, Speech, RAG) with phased rollout strategy
- **P3 — 短期可驗證**: 90-day POC plan with KPIs (≥30% review time reduction, ≥85% accuracy)
- **P4 — 推動承諾**: Commitments, timeline (2026-07-13 kickoff, 2026-07-25 written approval), budget source (城鄉發展基金)
- **附錄**: 7-module phased development roadmap (Phase 1–3), POC strategy, full TCO breakdown

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
