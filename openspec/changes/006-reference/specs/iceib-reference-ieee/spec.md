# Spec Delta

## Purpose

定義 `References`（`ICEIB paper/006-Reference.txt`）與全篇總裝檔（`ICEIB paper/main.txt`）的書目格式、引文溯源與端對端結構驗證契約。

## ADDED Requirements

### Requirement: IEEE 標準參考文獻著錄格式與溯源性
`006-Reference.txt` SHALL 使用 IEEE `\begin{thebibliography}{00}` 環境與 `\bibitem{b1}` 順序編號格式，所有書目條目（包含 WHO, HEI, MOENV 法規與開放資料集, 臺中市環保統計年報, 運動部調查及所有相關學術論文）MUST 可追溯至工作區已查證資料，不得臆測未經查證之作者姓名或 DOI。

#### Scenario: 核對書目欄位真實性與順序編號
- **WHEN** 逐筆核對 `006-Reference.txt` 與工作區佐證檔案
- **THEN** 每筆 `\bibitem` 均 MUST 符合 IEEE 會議引用格式（作者、雙引號篇名、斜體期刊／會議名、年份、DOI 或 `[Online]. Available: \url{...}`），且無任何憑空補齊之書目資訊

### Requirement: 全篇分段組裝與雙向交叉引用驗證
當 `main.txt` 組裝 `000-Abstract.txt` 至 `006-Reference.txt` 後，全篇 MUST 通過 100% 雙向引用一致性檢查（零遺漏 `\bibitem`、零未引用孤兒條目）、所有 `\ref` 解析成功、所有 LaTeX 環境與大括號配對正確，且無未跳脫特殊字元。

#### Scenario: 執行端對端 LaTeX 結構與引用檢查
- **WHEN** 對組裝後的 `main.txt` 及全部 `000`–`006` 分段檔執行結構驗證腳本
- **THEN** 腳本 MUST 回報 0 missing bibs、0 uncited bibs、0 missing labels、環境與大括號完全平衡，且無未跳脫之 `\&`、`\%` 或 `\_`
