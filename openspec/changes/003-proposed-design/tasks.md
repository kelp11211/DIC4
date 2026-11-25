# Tasks

## 1. Proposed Design 抽離與 PA–PM 結構整合

- [ ] 1.1 建立 `ICEIB paper/003-Proposed Design.txt` 並包含 `\section{Proposed Design}`，整併五大設計思維（Mindsets）與三大工程權衡（Trade-offs），並對齊設計目標與 `S1–S3` 使用情境（`PA–PC`, `PH`）。
- [ ] 1.2 完善八大編號模組 ①–⑧ 與系統架構圖（`PG`, TikZ `figure*`）、模組對照表、`QuerySpec`/`Observation`/`OfficialAQI`/`ForecastBundle`/`RuleEvidence`/`ResponseEnvelope` 六大契約，以及 2025 AQI 跨制度一致化說明（`PD–PF`）。

## 2. 流程圖、雙演算法、走查範例與數學形式化（PI–PM）

- [ ] 2.1 新增精簡 TikZ 控制與異常降級流程圖（`PI`, 單欄 `figure`，含品質檢查 Decision 與 Fallback 分支）及正文交叉引用，並驗證 `Algorithm 1`（`AirGuardAgent`）與 `Algorithm 2`（`TrainAndEvaluate`）連續行號與語法。
- [ ] 2.2 撰寫具體運動查詢走查範例（`PJ`：臺中晨跑時段比較與安全降級觸發）、貢獻收斂（`PK`）、評估銜接（`PL`）及嚴格因果時間窗與保守風險判定形式化公式（`PM`）。
- [ ] 2.3 檢查 `003-Proposed Design.txt` 全節 TikZ 節點名稱、數學符號與 LaTeX 特殊字元跳脫，確認無未閉合環境或未定義 `\ref`/`\cite`。

## Workflow follow-up

- 完成實作後執行 `openspec.cmd validate 003-proposed-design`，並於整篇審查通過後執行 `/opsx-archive 003-proposed-design`。
