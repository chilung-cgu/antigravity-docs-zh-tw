# Workflows (工作流程)

Workflows 定義了一套結構化的步驟或提示詞，用於自動化重複性任務。

## Running Workflows (執行工作流程)

您可以在對話輸入框中使用 `/workflow-name` (例如 `/security-audit`) 來啟動預定義的 Workflow。

## Creation & Format (建立與格式)

Workflows 是 Markdown 格式的檔案（上限 12,000 字元），包含標題、描述以及具體的執行步驟。

*   **Creation**: 透過 **Customization Panel (自定義面板)** -> **Workflows** -> **+ Global** 或 **+ Workspace** 建立。
*   **Nesting**: Workflows 可以呼叫其他 Workflows。
*   **Agent Generation**: 您可以請 Agent 根據目前的對話歷史記錄自動生成一個 Workflow。

---
導覽：[<- Rules](rules.md) | [Tools Overview ->](../tools/index.md)

---

> **原文參考**：[antigravity.google/docs/rules-workflows](https://antigravity.google/docs/rules-workflows)
