# Design

## Context

`ICEIB paper/main.txt` 目前包含整篇論文初稿。本設計將檔頭、作者區塊、摘要與關鍵字獨立抽離至 `ICEIB paper/000-Abstract.txt`，並將 `main.txt` 轉換為總裝主控檔，負責載入 `IEEEtran` 套件與依序引入 `000`–`006` 分段檔。

## Goals / Non-Goals

**Goals:**
- 使 `000-Abstract.txt` 專注承載標題、作者佔位符、A–F 單段式摘要與 `IEEEkeywords`。
- 確保 `main.txt` 與 `000-Abstract.txt` 在 Overleaf（將副檔名改為 `.tex` 或調整 `\input` 路徑）時可直接編譯無衝突。

**Non-Goals:**
- 不在摘要中放入圖表、數學推導或 `\cite` 引用（依 IEEE 會議摘要規範）。

## Decisions

### 1. 採主控檔載入套件＋分段檔純內容之拆檔模式
- **決策**：`\documentclass[conference,a4paper]{IEEEtran}` 與所有 `\usepackage{...}` 集中置於 `main.txt` 檔頭；`000-Abstract.txt` 僅放 `\title`、`\author`、`\maketitle`、`abstract` 與 `IEEEkeywords`。
- **理由**：避免各分段檔重複宣告 preamble 導致 LaTeX 編譯錯誤，也利於單獨審閱摘要。
- **替代方案**：每個檔案各自放完整 LaTeX 檔頭（無法直接被 `main.txt` `\input` 組裝，故不採用）。

### 2. 摘要長度與語態控制
- **決策**：維持 180–220 字單段式英文摘要，完整涵蓋 `A–F` 節點並使用預期成果語態。
- **理由**：符合 IEEE ICEIB 雙欄首頁版面空間配比與學術誠實要求。

## Risks / Trade-offs

- **[帶空白檔名在 `\input` 時相容性差異]** → `main.txt` 使用 `\input{"002-Related Work.txt"}` 雙引號寫法，並於設計註記中提醒 Overleaf 與 TeX Live 2020+ 環境相容性。
