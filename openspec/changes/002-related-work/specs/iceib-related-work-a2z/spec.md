# Spec Delta

## Purpose

定義 `II. Related Work`（`ICEIB paper/002-Related Work.txt`）的結構與內容契約，確保其落實 A2Z SOP `M–O` 三段式寫法、AI 與領域知識 50/50 均衡，並具備標準 8 欄文獻對照表。

## ADDED Requirements

### Requirement: Related Work 遵循 M–O 結構與 50/50 均衡原則
`002-Related Work.txt` SHALL 依循 `M`（大氣傳輸模式 → 統計與樹模型 → 深度時空網路）、`N`（MCP／ReAct 工具導向代理人、工具錯誤與事後幻覺之安全護欄新趨勢）及 `O`（整合比較與研究缺口推導）撰寫，且 MUST 涵蓋臺灣環境部 2025 新制 AQI 門檻與運動流行病學實證。

#### Scenario: 檢核技術與領域知識平衡覆蓋
- **WHEN** 審查 `002-Related Work.txt` 的子章節配置
- **THEN** 章節 MUST 同時包含空品預測／Agent 安全文獻（Chianese & Riccio, Joseph & Ganapathy, Lu & Lu, Houdou, Yao, Pan & Nipu, Ma et al., ToolHACE）與領域規範／公衛文獻（MOENV 2025 AQI 新制與開放資料集, Lo et al., WHO, BMC Medicine 2025）

### Requirement: 標準八欄文獻對照表與研究缺口歸納
章節 MUST 包含跨雙欄 `table*` 呈現 8 欄 `Article Summary Table`（`Ref./Source`、`Year`、`Problem`、`AI/Analytical Method`、`Domain Knowledge`、`Dataset`、`Key Findings`、`Limitations Addressed Here`），並於末尾歸納本研究聚焦之 Research Gap。

#### Scenario: 驗證八欄表格完整性與版面適配
- **WHEN** 檢查 `002-Related Work.txt` 的表格定義
- **THEN** 表格 MUST 具備精確 8 欄與完整 `\caption`／`\label`，採用適配 IEEE 雙欄寬度的 `tabularx` 設定，且清楚標示既有研究為何無法直接解決臺中測站級個人安全運動排程問題
