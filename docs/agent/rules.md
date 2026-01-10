# 規則 (Rules)

規則是用於引導代理行為的手動定義 Markdown 檔案（上限 12,000 字元）。您可以為特定專案或全域環境設定特定的行為準則。

## 如何定義規則

您可以透過**自定義面板 ("...")** -> **規則 (Rules)** -> **+ 全域 (Global)** 或 **+ 工作空間 (Workspace)** 來新增規則。

### 儲存位置
*   **全域規則 (Global)**：存儲於 `~/.gemini/GEMINI.md`。
*   **工作空間規則 (Workspace)**：存儲於專案目錄下的 `.agent/rules/`。

## 啟動方式

*   **手動 (Manual)**：在輸入框輸入 `@檔名` 來主動套用規則。
*   **總是開啟 (Always On)**：規則會應用於每一次互動。
*   **模型決策 (Model Decision)**：代理會根據自然語言描述自動決定何時套用規則。
*   **Glob 模式**：根據檔案路徑模式（例如 `src/**/*.ts`）自動套用。

---
導覽：[<- 設定](settings.md) | [工作流程 ->](workflows.md)

---

> **原文參考**：[antigravity.google/docs/rules-workflows](https://antigravity.google/docs/rules-workflows)
