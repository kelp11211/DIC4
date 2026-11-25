# Tasks

## 1. 相關研究模組化與 M–O 對齊

- [ ] 1.1 建立 `ICEIB paper/002-Related Work.txt` 並包含 `\section{Related Work}`，確認 `M`（預測方法由簡至繁分類）、`N`（MCP/ReAct 工具擴增與護欄新趨勢）及領域規範（MOENV 2025 新制 AQI、WHO、BMC Medicine 2025）達成 50/50 平衡。
- [ ] 1.2 核對並完善 8 欄 `Article Summary Table`（`table*`）與 `O`（Research Gap 轉折段落），確認欄位名稱、代表作年份、發現與限制與 [RELATED_WORK_REFACTOR.md](../../myplan/RELATED_WORK_REFACTOR.md) 一致。

## 2. 表格排版與引用檢查

- [ ] 2.1 檢查 `002-Related Work.txt` 中 `\tabularx` 欄位總寬與 LaTeX 特殊字元跳脫（`\&`、`\%`、`\_`），並確認表內所有 `\cite` 皆對應有效書目。

## Workflow follow-up

- 完成實作後執行 `openspec.cmd validate 002-related-work`，並於整篇審查通過後執行 `/opsx-archive 002-related-work`。
