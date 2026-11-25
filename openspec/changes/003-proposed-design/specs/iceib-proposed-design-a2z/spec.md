# Spec Delta

## Purpose

定義 `III. Proposed Design`（`ICEIB paper/003-Proposed Design.txt`）的技術與敘事契約，確保其完整實現 A2Z SOP `P` 階段（`PA–PM`）及 AirGuard AI 八大模組解耦架構。

## ADDED Requirements

### Requirement: 完整覆蓋 P 階段（PA–PM）設計要素
`003-Proposed Design.txt` SHALL 整合系統目標與三大情境 `S1–S3`（`PA–PC`）、設計思維與三項工程權衡（`PB`, `PH`）、八大編號模組 ①–⑧ 與資料契約（`PD–PF`）、系統架構圖（`PG`）與控制／異常降級流程圖（`PI`）、`Algorithm 1`（`AirGuardAgent`）與 `Algorithm 2`（`TrainAndEvaluate`）雙偽代碼（`PI`）、具體運動查詢走查範例（`PJ`）、貢獻對齊（`PK`）、評估銜接（`PL`）及時序因果與保守風險不等式形式化（`PM`）。

#### Scenario: 檢驗 PA–PM 與雙圖雙演算法齊備
- **WHEN** 檢查 `003-Proposed Design.txt` 內容
- **THEN** 章節 MUST 包含八大模組架構圖（`figure*`）、資料品質檢查與降級流程圖（`figure`）、兩段連續行號 `algorithm` 偽代碼、至少一個具體的 `S1/S2/S3` 走查範例，以及不讀取未來資訊之預測與區間保守準則公式

### Requirement: 2025 AQI 跨制度一致化與 Pydantic 契約一致性
設計說明 MUST 闡明 2024–2026 回測跨制度問題之解法（訓練目標採用物理濃度 $\mu\text{g/m}^3$，僅於模組 ⑥ 統一套用 2025-01-01 新制 AQI 門檻），並 SHALL 維持六大資料契約（`QuerySpec`, `Observation`, `OfficialAQI`, `ForecastBundle`, `RuleEvidence`, `ResponseEnvelope`）與五種輸出狀態（`ok`, `partial`, `needs_input`, `unavailable`, `out_of_horizon`）命名一致。

#### Scenario: 核對資料契約與 2025 AQI 處理機制
- **WHEN** 比對 `003-Proposed Design.txt` 與 `myplan/DESIGN.md`
- **THEN** 所有模組編號 ①–⑧、八個白名單工具名稱、六個資料契約名稱與五種終端狀態 MUST 完全一致
