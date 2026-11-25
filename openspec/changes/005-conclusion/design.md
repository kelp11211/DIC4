# Design

## Context

`005-Conclusion.txt` 對應論文 `\section{Conclusion}`（Section V），負責整合 W1–W6 實作路線、風險對策、四大系統限制與 A2Z SOP `W–Z` 結尾結構。

## Goals / Non-Goals

**Goals:**
- 建立 `ICEIB paper/005-Conclusion.txt`，明確映射 `W`（What proposed）、`X`（eXcel）、`Y`（Yields — Expected Outcomes & Roadmap）與 `Z`（Zen — Limitations, Risk Matrix & Future Work）。
- 維持全篇安全邊界與預期成果語態一致性。

**Non-Goals:**
- 不在結論引入前文未定義的新方法或未經實驗的定量宣稱。

## Decisions

### 1. 將 W1–W6 實作路線與風險控管表收斂於 Section V
- **決策**：將風險對策表（`tab:risks`）與六週里程碑納入 `V. Conclusion` 的 `Y` 與 `Z` 段落，並以四大限制明確界定適用範圍。
- **理由**：既保持五個頂層章節的簡潔，又能完整交代專案工程落地性。

## Risks / Trade-offs

- **[結論語氣容易不小心寫成「已完成驗證」]** → 於任務檢查加入語態審查，確保使用計畫／預期詞彙（"is designed to", "aims to", "future empirical execution will"）。
