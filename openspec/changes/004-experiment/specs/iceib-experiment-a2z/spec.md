# Spec Delta

## Purpose

定義 `IV. Experiment`（`ICEIB paper/004-Experiment.txt`）的評估設計與誠實聲明契約，確保論文精準對齊 A2Z SOP `Q–V` 與專案雙軌驗證架構。

## ADDED Requirements

### Requirement: Experiment 遵循 Q–V 六要素並定義雙軌評估指標
`004-Experiment.txt` SHALL 完整覆蓋 `Q`（`MAE`、`RMSE`、`Skill_MAE`、高污染召回率、工具正確率／來源完整率／規則一致率／降級率／醫療零越權／延遲 P50-P95）、`R`（Persistence、Seasonal Naive、Ridge/RF/XGBoost/LSTM 與 Rule-only 對照）、`S`（2024–2026 臺中測站與 70/15/15 時間切分）、`T`（Rolling-origin 調參與特徵／規則／不確定性消融規劃）、`U`（預期結果判讀準則與外部文獻參考區間）及 `V`（≥30 情境 7 大風險類別驗證表）。

#### Scenario: 核對 Q–V 指標與測試類別齊備性
- **WHEN** 檢視 `004-Experiment.txt` 內容
- **THEN** 章節 MUST 包含 `Skill_MAE` 數學式、Track B 七類風險測試表（含假前提、醫療越權、資訊不足、API 失敗、超時距、工具矛盾、提示注入），且每個 `Q–V` 項目皆有明確對應段落

### Requirement: 嚴禁虛構未經執行之實驗數據
章節首段 MUST 顯式聲明系統尚處於架構與實驗設計階段（未執行訓練與測試），所有目標數值均標記為「Expected Outcomes / Targets」，且外部文獻數據（如雲林 ST-GCN MAE $2.711~\mu\text{g/m}^3$ 與西屯 EEMD-GRU 95.39\%）MUST 明確註記僅作參考範圍。

#### Scenario: 審查實驗數據誠實性
- **WHEN** 檢查 `004-Experiment.txt` 中所有量化指標
- **THEN** 文本 MUST NOT 出現任何偽造的 AirGuard AI 實測 MAE、RMSE 或準確率表格，且若 ML 未勝過 Persistence 須明文承諾如實報告
