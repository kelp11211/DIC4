# Proposal

## Why

為使 IEEE ICEIB 研討會論文具備模組化撰寫與逐節審查能力，需將摘要與 IEEE 版面骨架獨立為獨立規格單元，嚴格對齊 [iceib.asia](https://www.iceib.asia/) 雙欄研討會排版規範與 A2Z SOP 的 `A–F` 六段式科研摘要結構。

## What Changes

- 建立獨立檔頭與摘要模組 `ICEIB paper/000-Abstract.txt`，規範 `\documentclass[conference,a4paper]{IEEEtran}`、單盲作者佔位符、英文 `abstract` 與 `IEEEkeywords`。
- 依據 `A–F`（Attention Getter, But, Cure, Development, Experiments, Findings）撰寫或精煉單段式摘要，並確保在提案設計階段僅呈預期成果（Expected Outcomes），不虛構實證數據。
- 規範 `ICEIB paper/main.txt` 主控檔與各分節檔案（`000-Abstract.txt` 至 `006-Reference.txt`）之組裝介面與 LaTeX 套件共用邊界。

## Capabilities

### New Capabilities
- `iceib-abstract-a2z`: 規範符合 IEEE ICEIB 雙欄格式與 A2Z SOP `A–F` 結構的論文檔頭、摘要與關鍵字模組，以及主文件組裝契約。

### Modified Capabilities
<!-- None -->

## Impact

- **目標產出檔案**：`ICEIB paper/000-Abstract.txt`、`ICEIB paper/main.txt`（總裝入點）。
- **參考依據**：`myplan/A2Z outline example.pdf`、`myplan/AirGuard AI 完整 A2Z 科研提案資訊圖表.png`、`myplan/空品決策代理人.md`。
