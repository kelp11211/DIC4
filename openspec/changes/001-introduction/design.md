# Design

## Context

`001-Introduction.txt` 承載論文第一節 `\section{Introduction}`。除既有動機與貢獻外，依整體五節架構決策，原獨立章節中的 SWOT 批判與研究缺口整合至緒論的 `J` 節點，確保從公衛背景（`G`）一路推導至本研究貢獻（`K`）與文章組織（`L`）。

## Goals / Non-Goals

**Goals:**
- 將 `I. Introduction` 獨立為 `ICEIB paper/001-Introduction.txt`，對應 `G–L` 六個寫作節點。
- 強化 `J` 節點的 SWOT 精煉評析與 Research Gap 敘述，並使 `L` 節點準確對應 `Section II`–`Section V`。

**Non-Goals:**
- 不在緒論重複鋪陳八大模組演算法細節（留待 `003-Proposed Design.txt`）。

## Decisions

### 1. 將 SWOT 分析精煉融入 `I. Introduction` 的 `J` 節點
- **決策**：在 `I`（既有三大類方法概述）之後，以精煉學術散文或簡明比較表完成 `J`（SWOT 優劣批判與 Research Gap），不另設獨立頂層章節。
- **理由**：完整遵循 `A2Z outline example.pdf` 之 `G–L` 編排，並維持 ICEIB 論文緊湊篇幅。
- **替代方案**：把 SWOT 放到 `II. Related Work`（會與 `M–O` 重複，故不採用）。

## Risks / Trade-offs

- **[臺中 AQI > 100 天數屬自行推算]** → 明確標註「derived from the 2025 Taichung Environmental Protection Statistical Yearbook」，遵守佐證資料使用提醒。
