# Modes (模式)

當啟動新的 Agent 對話時，使用者可以選擇不同的 Mode。此外，Antigravity 的核心 Workflow 也遵循「Planning, Execution, Verification」的生命週期。

## Conversation Modes (對話模式)

### Planning Mode
Agent 在執行任務前會進行規劃。適用於深度研究、複雜任務或協作工作。在此模式下，Agent 會將工作組織成 **Task groups**，產出 **Artifacts**，並採取其他步驟進行徹查、思考與規劃，以確保最佳品質。

### Fast Mode
Agent 將直接執行任務。適用於可以快速完成的簡單任務，例如重新命名變數、啟動幾個 Bash 命令或其他較小的分區任務。當速度是重要因素且任務足夠簡單、不必擔心品質下降時，此模式非常有用。

## Agent Lifecycle (代理生命週期)

Antigravity 透過強調以下階段，使 Agent 能夠跨多個介面自主運行：

*   **Planning (規劃)**：建立結構化計畫與 Task groups。
*   **Execution (執行)**：同步控制 Editor、Terminal 與 Browser 介面。

---
導覽：[<- Models](models.md) | [Settings ->](settings.md)

---

> **原文參考**：[antigravity.google/docs/agent-modes-settings](https://antigravity.google/docs/agent-modes-settings)
