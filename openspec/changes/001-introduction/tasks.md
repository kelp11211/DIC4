# Tasks

## 1. 緒論模組抽離與 G–L 結構重構

- [ ] 1.1 建立 `ICEIB paper/001-Introduction.txt` 並包含 `\section{Introduction}`，確保所有量化背景數據（HEI 2024、WHO、體育署 2025、BMC Medicine 2025、臺中 2025 測站推算、Draelos 2026、Omar 2025）皆附有效 `\cite` 鍵值。
- [ ] 1.2 依 `G–L` 順序檢視並強化 `J`（SWOT 批判與 Research Gap 推導）、`K`（四大安全防線與三大預期貢獻）及 `L`（對齊 `Section II`–`Section V` 之組織說明），透過文字檢核確認六節點無一遺漏。

## 2. 格式與引用一致性驗證

- [ ] 2.1 檢查 `001-Introduction.txt` 的 LaTeX 語法（跳脫字元 `\%`、`\&`、環境配對）與所有 `\cite{...}` 鍵值是否可於 `006-Reference.txt` 解析。

## Workflow follow-up

- 完成實作後執行 `openspec.cmd validate 001-introduction`，並於整篇審查通過後執行 `/opsx-archive 001-introduction`。
