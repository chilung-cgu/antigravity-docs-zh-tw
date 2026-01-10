# 模式 (Modes)

當啟動新的智能代理 (Agent) 對話時，使用者可以選擇不同的模式。此外，Antigravity 的核心工作流程也遵循「規劃、執行、驗證」的生命週期。

## 對話模式

### 規劃模式 (Planning Mode)
代理在執行任務前會進行規劃。適用於深度研究、複雜任務或協作工作。在此模式下，代理會將工作組織成**任務組 (Task groups)**，產出**產出物 (Artifacts)**，並採取其他步驟進行徹查、思考與規劃，以確保最佳品質。

### 快速模式 (Fast Mode)
代理將直接執行任務。適用於可以快速完成的簡單任務，例如重新命名變數、啟動幾個 Bash 命令或其他較小的分區任務。當速度是重要因素且任務足夠簡單、不必擔心品質下降時，此模式非常有用。

## 代理生命週期 (規劃、執行、驗證)

Antigravity 透過強調以下階段，使代理能夠跨多個介面自主運行：

*   **規劃 (Planning)**：建立結構化計畫與任務組。
*   **執行 (Execution)**：同步控制編輯器、終端機與瀏覽器介面。
*   **驗證 (Verification)**：檢查代理工作的結果，以確保更高層級的溝通與品質（通常使用瀏覽器子代理或審閱產出物）。

---
導覽：[<- 模型](models.md) | [設定 ->](settings.md)

---

> **原文參考**：[antigravity.google/docs/agent-modes-settings](https://antigravity.google/docs/agent-modes-settings)
