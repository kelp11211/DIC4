# Proposal

## Why

實驗與評估規劃（Experiment）必須嚴謹定義時序防洩漏回測與 Agent 安全性測試，並在提案尚未實際執行前嚴守學術誠實規範。將其獨立為 `004-experiment` 規格單元，可完整對應 A2Z SOP 的 `Q–V` 結構，將 Track A（預測軌）與 Track B（代理人軌）的指標、基線、環境設置、調參消融與驗證目標規格化。

## What Changes

- 建立獨立章節檔案 `ICEIB paper/004-Experiment.txt`，對應論文 `\section{Experiment}`。
- 依循 `Q–V` 結構展開：量化與質化指標（`Q`）、對比基線與候選模型（`R`）、2024–2026 臺中測站與 70/15/15 切分設置（`S`）、滾動原點超參數調整與消融實驗設計（`T`）、預期分析與外部參考基準區間（`U`），以及 ≥30 情境安全驗證矩陣與系統品質驗收（`V`）。
- 強制加入方法論透明聲明，杜絕任何未經執行的模型結果宣稱。

## Capabilities

### New Capabilities
- `iceib-experiment-a2z`: 規範遵循 A2Z SOP `Q–V` 結構與雙軌驗收框架（Track A + Track B）的實驗設計章節，並落實提案階段不虛構實驗結果的學術誠實護欄。

### Modified Capabilities
<!-- None -->

## Impact

- **目標產出檔案**：`ICEIB paper/004-Experiment.txt`（由 `ICEIB paper/main.txt` 載入）。
- **參考依據**：`myplan/DESIGN.md`、`myplan/AirGuard_AI_Final_Proposal.docx`、`myplan/空污 × 戶外運動 AI Agent 提案：研究佐證資料.md`、`myplan/A2Z outline example.pdf`。
