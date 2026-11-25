# Tasks

## 1. IEEE 書目抽離與溯源核對

- [ ] 1.1 建立 `ICEIB paper/006-Reference.txt`，封裝 `\begin{thebibliography}{00} ... \end{thebibliography}` 與所有 `\bibitem{b1}`–`\bibitem{bN}` 條目。
- [ ] 1.2 逐筆核對 `006-Reference.txt` 與 [研究佐證資料.md](../../myplan/%E7%A9%BA%E6%B1%A1%20%C3%97%20%E6%88%B6%E5%A4%96%E9%81%8B%E5%8B%95%20AI%20Agent%20%E6%8F%90%E6%A1%88%EF%BC%9A%E7%A0%94%E7%A9%B6%E4%BD%90%E8%AD%89%E8%B3%87%E6%96%99.md) 及 `AirGuard_AI_Final_Proposal.docx`，確認無未查證作者、年份、DOI 或 URL。

## 2. 總裝組裝與端對端 LaTeX 驗證

- [ ] 2.1 確認 `ICEIB paper/main.txt` 正確引入 `000-Abstract.txt` 至 `006-Reference.txt`，執行展開式 PowerShell 驗證腳本確認 0 missing bibs、0 uncited bibs、0 missing labels、環境與大括號完全平衡且無未跳脫特殊字元。

## Workflow follow-up

- 完成實作並確認全部 000–006 變更通過驗證後，依序執行 `/opsx-archive 000-abstract` 至 `/opsx-archive 006-reference` 將論文規格歸檔至 `openspec/specs/`。
