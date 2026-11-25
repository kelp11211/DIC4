# Spec Delta

## Purpose

定義 `I. Introduction`（`ICEIB paper/001-Introduction.txt`）的寫作契約，確保在 IEEE 英文會議語體下完整貫徹 A2Z SOP `G–L` 六段式結構與 AirGuard AI 核心安全邊界。

## ADDED Requirements

### Requirement: 緒論遵循 G–L 六段式論證脈絡
`001-Introduction.txt` SHALL 依序涵蓋 `G`（全球空污負擔與臺灣／臺中運動現況）、`H`（運動效益折損、官方預報解析度斷層、LLM 幻覺／諂媚／醫療越權三大挑戰）、`I`（既有三大類方法脈絡）、`J`（SWOT 批判性評估與 Research Gap 推導）、`K`（三大預期貢獻與四大安全防線）以及 `L`（Section II–V 章節組織預告）。

#### Scenario: 驗證 G–L 結構與 L 組織段對齊
- **WHEN** 檢查 `001-Introduction.txt` 的段落邏輯與文末組織預告
- **THEN** 段落 MUST 完整對應 `G` 至 `L` 六節點，且 `L` 節點列舉的章節編號 MUST 精確對應 `Section II`（Related Work）、`Section III`（Proposed Design）、`Section IV`（Experiment）與 `Section V`（Conclusion）

### Requirement: 緒論實證數據溯源與四大安全防線
緒論引用的健康與空品統計 MUST 與工作區已查證佐證資料一致，並 SHALL 明示四大核心安全防線（測站尺度非街道暴露、PM2.5 預測非官方 AQI、1–6h 不可外推隔日、不提供個人醫療診斷）。

#### Scenario: 核對公衛數據與四大防線陳述
- **WHEN** 檢視緒論內之量化統計與系統定位描述
- **THEN** HEI 2024（810 萬死亡）、BMC Medicine 2025（25 μg/m³ 門檻效益腰斬）、臺中 2025 測站推算（18–31 天 AQI > 100）、Draelos 2026（5%–13% 不安全回答）與 Omar 2025（50%–82% 假前提附和）等數據 MUST 附有正確 `\cite` 鍵值，且四大防線皆明確表述
