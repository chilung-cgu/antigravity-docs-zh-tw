# 工作流程 (Workflows)

工作流程定義了一套結構化的步驟或提示詞，用於自動化重複性任務。

## 執行工作流程

您可以在對話輸入框中使用 `/工作流程名稱` (例如 `/security-audit`) 來啟動預定義的工作流程。

## 建立與格式

工作流程是 Markdown 格式的檔案（上限 12,000 字元），包含標題、描述以及具體的執行步驟。

*   **建立方式**：透過**自定義面板** -> **工作流程 (Workflows)** -> **+ 全域** 或 **+ 工作空間** 建立。
*   **巢狀執行 (Nesting)**：工作流程可以呼叫其他工作流程。
*   **代理生成 (Agent Generation)**：您可以請代理根據目前的對話歷史記錄自動生成一個工作流程。

---
導覽：[<- 規則](rules.md) | [工具概述 ->](../tools/index.md)

---

> **原文參考**：[antigravity.google/docs/rules-workflows](https://antigravity.google/docs/rules-workflows)
