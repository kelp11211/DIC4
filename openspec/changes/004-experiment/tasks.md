# Tasks

## 1. Experiment 模組化與 Q–V 雙軌設計

- [ ] 1.1 建立 `ICEIB paper/004-Experiment.txt` 並包含 `\section{Experiment}`，於開頭顯式標註方法論透明聲明（目前為實驗設計與協議規格階段，尚未執行實際訓練與測試）。
- [ ] 1.2 撰寫 Track A（`Q–T`：`MAE`、`RMSE`、`Skill_MAE` 公式、Persistence/Seasonal Naive 基線、2024–2026 臺中測站 70/15/15 切分、Rolling-origin 超參數調整與特徵／規則消融規劃）。
- [ ] 1.3 撰寫 Track B 與預期結果分析（`Q, U, V`：Rule-only 對照設計、≥30 情境 7 類安全測試表與預期目標，並將外部文獻數據如 Yunlin ST-GCN 與 Xitun EEMD-GRU 明確區隔為參考範圍）。

## 2. 誠實性與格式檢查

- [ ] 2.1 檢查 `004-Experiment.txt` 無任何虛構 AirGuard AI 測試數值，且所有公式、表格欄位與 `\cite`/`\label` 均符合 `IEEEtran` 雙欄排版規範。

## Workflow follow-up

- 完成實作後執行 `openspec.cmd validate 004-experiment`，並於整篇審查通過後執行 `/opsx-archive 004-experiment`。
