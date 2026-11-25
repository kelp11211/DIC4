# Proposal

## Why

參考文獻（References）與跨檔案總裝驗證是確保 IEEE ICEIB 投稿合規的最後關卡。將其獨立為 `006-reference` 規格單元，可系統化控管 `ICEIB paper/006-Reference.txt` 內所有 IEEE `\bibitem` 書目條目與工作區佐證資料的一致性，並負責驗證 `ICEIB paper/main.txt` 組裝 `000`–`006` 全數分段檔後的 LaTeX 結構與交叉引用完整性。

## What Changes

- 建立獨立章節檔案 `ICEIB paper/006-Reference.txt`，封裝符合 IEEE 標準格式的 `\begin{thebibliography}{00} ... \end{thebibliography}`。
- 核對每一筆書目條目與工作區佐證文件（`空污 × 戶外運動 AI Agent 提案：研究佐證資料.md` 與 `AirGuard_AI_Final_Proposal.docx`），確保作者、年份、篇名、期刊／會議名稱、DOI 與官方 URL 正確無誤且無臆測欄位。
- 完成 `ICEIB paper/main.txt` 對 `000-Abstract.txt` 至 `006-Reference.txt` 的總裝與全篇自動化檢查（環境配對、大括號平衡、`\cite` 與 `\bibitem` 100% 雙向匹配、`\ref`/`\label` 解析及特殊字元跳脫）。

## Capabilities

### New Capabilities
- `iceib-reference-ieee`: 規範 `006-Reference.txt` 之 IEEE 書目著錄格式、全篇引用溯源一致性，以及 `main.txt` 組裝 000–006 分段檔後的端對端 LaTeX 語法驗證契約。

### Modified Capabilities
<!-- None -->

## Impact

- **目標產出檔案**：`ICEIB paper/006-Reference.txt`、`ICEIB paper/main.txt`（總裝驗證）。
- **參考依據**：`myplan/空污 × 戶外運動 AI Agent 提案：研究佐證資料.md`、`myplan/AirGuard_AI_Final_Proposal.docx`、`myplan/README.md`。
