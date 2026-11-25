# Spec Delta

## Purpose

定義 `V. Conclusion`（`ICEIB paper/005-Conclusion.txt`）的寫作契約，確保其遵循 A2Z SOP `W–Z` 結構，誠實收束預期成果並清楚界定系統限制與未來實驗方向。

## ADDED Requirements

### Requirement: Conclusion 遵循 W–Z 四段式收束結構
`005-Conclusion.txt` SHALL 依循 `W`（What proposed：回顧研究動機與職責分離架構）、`X`（eXcel：闡述最適合的短期運動排程與高風險防護場景）、`Y`（Yields：簡述預期的雙軌產出與 W1–W6 實作交付規劃）及 `Z`（Zen：交代四大已知限制、主要風險控管矩陣與未來 $\text{O}_3$ 整合／使用者研究方向）完成收束。

#### Scenario: 檢驗 W–Z 結構與四大限制一致性
- **WHEN** 檢視 `005-Conclusion.txt` 的段落結構
- **THEN** 文本 MUST 完整涵蓋 `W–Z` 四要素、風險緩解摘要表與 W1–W6 路線圖，且 MUST 清楚列出測站代表性、不確定性隨時距擴大、非醫療器材與臺中區域限制等四項邊界

### Requirement: 結論不得超前宣稱未驗證成效
結論所述及的模型增益、安全性與系統效益 MUST 使用預期或目標語氣（e.g., "is expected to", "aims to"），嚴禁以既成事實口吻宣稱尚未執行之回測結果。

#### Scenario: 審查結論語氣與預期成果邊界
- **WHEN** 檢查 `005-Conclusion.txt` 之語句描述
- **THEN** 所有與尚未執行實驗相關的產出均 MUST 明確標示為計畫或預期成果，無已達成準確率之虛假表述
