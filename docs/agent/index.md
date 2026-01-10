# 智能代理 (Agent)

代理是 Google Antigravity 內最主要的 AI 功能。它是一個由尖端大語言模型 (LLM) 驅動的多步驟推理系統，能夠對您現有的程式碼進行推理、使用各種工具（包括瀏覽器），並透過任務 (Tasks)、產出物 (Artifacts) 等方式與使用者溝通。

## 核心組件

*   **推理模型 (Reasoning model)**：提供智能基礎的底層大語言模型。
*   **工具 (Tools)**：代理可用於與環境互動的能力。
*   **產出物 (Artifacts)**：程式碼與文件的專業輸出格式。
*   **知識庫 (Knowledge)**：代理可存取的上下文與資訊。

## 自定義

*   **代理模式 / 設定 (Agent Modes / Settings)**：代理行為的組態選項。
*   **MCP**：Model Context Protocol 整合。
*   **規則 / 工作流程 (Rules / Workflows)**：針對日常任務的預定義指令集。

您可以啟動多個代理對話，包括併行執行。您可以透過代理管理器中的「右鍵點擊 > 刪除對話」或點擊編輯器代理面板中的垃圾桶圖示來刪除代理對話。

---
導覽：[<- 快速入門](../getting-started/index.md) | [模型 ->](models.md)

---

> **原文參考**：[antigravity.google/docs/agent](https://antigravity.google/docs/agent)
