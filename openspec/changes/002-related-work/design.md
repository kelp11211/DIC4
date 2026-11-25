# Design

## Context

`002-Related Work.txt` 對應 `\section{Related Work}`，必須依照 A2Z SOP `M–O` 完成技術文獻與領域知識 50/50 均衡論述，並以 8 欄 `Article Summary Table` 收斂出核心研究缺口。

## Goals / Non-Goals

**Goals:**
- 將相關研究抽離至 `ICEIB paper/002-Related Work.txt`，維持 `M`（預測方法演進）、`N`（工具導向 Agent 與安全護欄新趨勢）、`O`（8 欄文獻對照表與 Research Gap 轉折）。
- 確保 `table*` 跨雙欄表格排版清晰、無欄位重疊或超過邊界。

**Non-Goals:**
- 不在此節重複詳述 AirGuard AI 自身模組或偽代碼（屬於 `003-Proposed Design.txt`）。

## Decisions

### 1. 採三個子章節對應 `M`、`N` 與領域基礎，並以 `table*` 總結 `O`
- **決策**：`II.A` 覆蓋預測模型三代演進（`M`）；`II.B` 覆蓋工具擴增 Agent 與護欄安全趨勢（`N`）；`II.C` 深入臺灣 MOENV 2025 AQI 新制與運動醫學知識（Domain 50%）；`II.D` 搭配 `table*` 完成 8 欄比較與 Research Gap（`O`）。
- **理由**：兼顧 AI 技術 50% 與領域知識 50% 的審稿要求，並讓 8 欄比較表順暢置頂於雙欄頁面。

## Risks / Trade-offs

- **[8 欄表格文字過密導致超出行寬]** → 使用 `\scriptsize`、`\tabularx` 搭配固定寬度 `p{...}` 與 `\renewcommand{\arraystretch}{1.15}` 控制列高與換行。
