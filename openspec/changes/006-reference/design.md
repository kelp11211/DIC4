# Design

## Context

`006-Reference.txt` 封裝整篇論文的 IEEE 參考文獻列表（`\begin{thebibliography}{00}`），而本變更同時負責在所有分段檔案就緒後，對 `ICEIB paper/main.txt` 進行最終的跨檔結構與引用驗證。

## Goals / Non-Goals

**Goals:**
- 將書目抽離為 `ICEIB paper/006-Reference.txt`，所有條目按正文出現順序編號並嚴格遵守 IEEE 引用格式。
- 確認每一筆參考文獻均可追溯至工作區現有文件，無任何臆測欄位。
- 完成 `main.txt` 對 `000`–`006` 全部檔案的總裝與自動化驗證。

**Non-Goals:**
- 不引入工作區未曾查證過的外來假引文。

## Decisions

### 1. 跨分段檔自動化驗證策略
- **決策**：在執行總裝驗證時，透過 PowerShell 讀取 `main.txt` 並展開所有 `\input{...}` 內容，再對展開後的完整文本檢查環境配對、大括號、`\cite` vs `\bibitem`、`\ref` vs `\label` 與未跳脫字元。
- **理由**：即使沒有本地 `pdflatex`，仍能以程式化方式確保分段檔組裝後具備 100% 語法與引用一致性。

## Risks / Trade-offs

- **[分段各自撰寫後出現 `\cite{bX}` 編號重複或遺漏]** → 規定所有 `\bibitem{bN}` 統一由 `006-Reference.txt` 維護，並由驗證腳本確認 0 missing / 0 uncited。
