# Proposal

## Why

`III. Proposed Design` 是整篇論文佔比與技術密度最高的核心章節，須將原本散落的系統設計理念、八大模組架構、資料契約、流程圖與雙演算法依 A2Z SOP 的 `P` 階段（`PA–PM` 十三項要素）嚴謹整合。將其獨立為 `003-proposed-design`，可確保架構設計、數學形式化與範例走查皆符合審查標準。

## What Changes

- 建立獨立章節檔案 `ICEIB paper/003-Proposed Design.txt`，對應論文 `\section{Proposed Design}`。
- 整併原獨立的系統設計原則與三大工程權衡，並完整對齊 `PA–PM` 要素：設計目標與情境（`PA–PC`）、八大模組 ①–⑧ 與資料契約（`PD–PF`）、系統架構圖與異常降級流程圖（`PG`, `PI`）、安全守門機制（`PH`, `PK`）、`Algorithm 1` 與 `Algorithm 2` 偽代碼（`PI`）、臺中晨跑走查範例（`PJ`）、模擬銜接（`PL`）及時序防洩漏／保守判定形式化（`PM`）。

## Capabilities

### New Capabilities
- `iceib-proposed-design-a2z`: 規範遵循 A2Z SOP `P (PA–PM)` 結構的系統設計章節，涵蓋八大模組 ①–⑧、雙 TikZ 圖表、Pydantic 契約、2025 AQI 跨制度處理、雙演算法與案例走查。

### Modified Capabilities
<!-- None -->

## Impact

- **目標產出檔案**：`ICEIB paper/003-Proposed Design.txt`（由 `ICEIB paper/main.txt` 載入）。
- **參考依據**：`myplan/DESIGN.md`、`myplan/AirGuard_AI_Final_Proposal.docx`、`myplan/A2Z outline example.pdf`、`myplan/AirGuard AI 完整 A2Z 科研提案資訊圖表.png`。
