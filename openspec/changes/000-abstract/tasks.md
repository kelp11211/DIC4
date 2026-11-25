# Tasks

## 1. 摘要與主控檔架構拆分

- [ ] 1.1 建立 `ICEIB paper/000-Abstract.txt`，移入 `\title`、三位作者 `\IEEEauthorblockN`/`\IEEEauthorblockA` 佔位符、`\maketitle`、`\begin{abstract}` 與 `\begin{IEEEkeywords}`，並驗證無獨立 `\documentclass` 重複宣告。
- [ ] 1.2 更新 `ICEIB paper/main.txt` 保留完整 `IEEEtran` (`a4paper`) preamble，並透過 `\input` 依序引入 `000-Abstract.txt` 至 `006-Reference.txt`，驗證大括號與環境配對無誤。

## 2. A–F 寫作規範與誠實檢查

- [ ] 2.1 逐項檢核 `000-Abstract.txt` 摘要文字是否完整覆蓋 `A`（25 μg/m³ 與全球空污動機）、`B`（預報與 LLM 缺口）、`C`（AirGuard AI）、`D`（MOENV 資料與 1/3/6h 模型）、`E`（雙軌回測與 30 情境）與 `F`（Expected Outcomes），驗證摘要內無 `\cite` 且無虛構數據。

## Workflow follow-up

- 完成實作並確認組裝結果後，執行 `openspec.cmd validate 000-abstract` 並透過 `/opsx-archive 000-abstract` 歸檔。
