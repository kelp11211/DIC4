# Spec Delta

## Purpose

規範 IEEE ICEIB 研討會論文的檔頭設定、作者資訊與符合 A2Z SOP（`A–F`）的英文摘要及關鍵字模組，並定義 `main.txt` 組裝各分段檔的版面契約。

## ADDED Requirements

### Requirement: IEEE ICEIB 版面檔頭與作者區塊規格
系統之論文主控與摘要模組 MUST 採用 `\documentclass[conference,a4paper]{IEEEtran}`，設定 A4 雙欄單倍行距、不插入手動頁碼，並提供可替換的三位作者資訊區塊與無編號腳註聲明（標註現階段為設計與實驗規劃階段）。

#### Scenario: 檢核 IEEEtran 檔頭與主控組裝介面
- **WHEN** 檢視 `ICEIB paper/main.txt` 與 `ICEIB paper/000-Abstract.txt`
- **THEN** 主控檔 MUST 宣告 `IEEEtran` 會議類別與共用套件，並透過 `\input` 依序載入 `000-Abstract.txt` 至 `006-Reference.txt`

### Requirement: 摘要 A–F 六段式科研故事完整性
`000-Abstract.txt` SHALL 在單一精煉英文段落內依序涵蓋 `A`（Attention Getter）、`B`（But）、`C`（Cure）、`D`（Development）、`E`（Experiments）與 `F`（Findings / Expected Outcomes），並配合 `IEEEkeywords` 列出 4–7 個領域與技術關鍵字。

#### Scenario: 驗證 A–F 要素與學術誠實邊界
- **WHEN** 審閱摘要段落內容
- **THEN** 摘要 MUST 交代 `25 μg/m³` 運動效益折損、既有預報與 LLM 缺口、AirGuard AI 解耦架構、MOENV 資料與 1/3/6h 模型設計、雙軌回測與 30 情境規劃，且 MUST NOT 宣稱未經執行的模型準確率
