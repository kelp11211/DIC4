# Design

## Context

`003-Proposed Design.txt` 對應論文 `\section{Proposed Design}`（Section III）。為了完整滿足使用者指定的五節結構與 A2Z SOP `P` 階段（`PA–PM` 十三個細項），需將原本獨立的「Design Principles」整併進本節的設計基礎與權衡論述，並補足初稿缺少的系統流程圖（Flowchart）、具體情境走查（`PJ`）與形式化防洩漏／保守判定準則（`PM`）。

## Goals / Non-Goals

**Goals:**
- 將提案設計完整抽離至 `ICEIB paper/003-Proposed Design.txt`。
- 使 Section III 逐一對應 `PA–PM`：目標與情境 `S1–S3`（`PA–PC`）、五大思維與三大權衡（`PB`, `PH`）、八大模組 ①–⑧ 與 Pydantic 契約（`PD–PF`）、系統架構圖 `figure*`（`PG`）、控制與異常降級流程圖 `figure`（`PI`）、`Algorithm 1` & `Algorithm 2`（`PI`）、臺中晨跑走查範例（`PJ`）、創新貢獻對齊（`PK`）、模擬銜接（`PL`）及預測／保守區間數學形式化（`PM`）。

**Non-Goals:**
- 不在本節放入真實模型測試數值或實作程式原始碼。

## Decisions

### 1. 同時保留八大模組架構圖（`figure*`）與控制流程圖（`figure`）
- **決策**：架構圖以跨雙欄 `figure*` 呈現 ①–⑧ 與四個資料／規則／稽核儲存層；流程圖以單欄 `figure` 呈現 `Input -> Planner -> Retrieval -> Quality Check -> ML -> Domain Rules -> Decision -> Output` 及 `Exception/Fallback` 降級分支。
- **理由**：對應 `AirGuard AI 完整 A2Z 科研提案資訊圖表.png` 第 4.2 與 4.3 節之雙圖規範，皆採自包含 TikZ 語法以確保 Overleaf 免外部圖片即可編譯。

### 2. 以 `PJ` 走查案例與 `PM` 數學式補足 PA–PM 完整度
- **決策**：新增一組具體的臺中忠明站晨跑查詢（含一般族群時段比較、敏感族群與 >6h 降級分支）作為 `PJ` 範例，並補充過去資訊集合 $\mathcal{F}_{s,t}$ 與誤差帶跨越門檻時的保守判定準則作為 `PM`。
- **理由**：完全覆蓋 `A2Z outline example.pdf` 的 `PA–PM` 要求。

## Risks / Trade-offs

- **[TikZ 雙圖與雙演算法導致 Section III 篇幅過長]** → 單欄流程圖採精簡垂直流設計、演算法採 `\scriptsize`，並將實作介面細節精煉納入表格中。
