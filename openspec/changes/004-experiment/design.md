# Design

## Context

`004-Experiment.txt` 對應論文 `\section{Experiment}`（Section IV），須將原本分散於系統評估與預期成果的內容收斂並完整對齊 A2Z SOP `Q–V`（Quality/Quantity, Related methods, Setup, Tuning, Useful results/analysis, Verification）。

## Goals / Non-Goals

**Goals:**
- 將雙軌實驗與評估設計抽離至 `ICEIB paper/004-Experiment.txt`。
- 明確將 `Q–V` 六要素與 Track A（PM2.5 預測回測）及 Track B（≥30 情境 Agent 測試）一一映射，補充原本欠缺的「超參數調整與消融實驗配置（`T`）」細節。
- 徹底守住學術誠實原則，將所有未執行結果限定為 Expected Outcomes / Targets。

**Non-Goals:**
- 不得在本變更階段執行模型訓練或產生虛構的實驗數據表。

## Decisions

### 1. 以雙軌表單與明確 `Q–V` 對應架構呈現未執行實驗規範
- **決策**：將 Section IV 組織為方法論透明聲明、Track A（`Q, R, S, T`：指標與基線、資料切分、滾動原點調參與消融實驗）、Track B（`Q, R, V`：Rule-only vs Agent+ML+Rules、7 大類別 ≥30 情境測試表）及預期產出與外部參考基準定位（`U`）。
- **理由**：使審查者一眼掌握完整可重現的實驗設計，同時完全避免未實作階段的學術不實風險。

## Risks / Trade-offs

- **[審查者誤將外部文獻數據當成本文實測成果]** → 於表格與正文中使用明顯標記（e.g., "External contextual benchmark only — not directly comparable"），並於首段放透明聲明。
