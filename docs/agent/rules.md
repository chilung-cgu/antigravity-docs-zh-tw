# Rules (規則)

Rules 是用於引導 Agent 行為的手動定義 Markdown 檔案（上限 12,000 字元）。您可以為特定專案或全域環境設定特定的行為準則。

## Defining Rules (定義規則)

您可以透過 **Customization Panel (自定義面板)** (`...`) -> **Rules** -> **+ Global** 或 **+ Workspace** 來新增規則。

### Storage Location (儲存位置)
*   **Global Rules**: 存儲於 `~/.gemini/GEMINI.md`。
*   **Workspace Rules**: 存儲於專案目錄下的 `.agent/rules/`。

## Activation (啟動方式)

*   **Manual**: 在輸入框輸入 `@filename` 來主動套用 Rules。
*   **Always On**: Rules 會應用於每一次互動。
*   **Model Decision**: Agent 會根據自然語言描述自動決定何時套用 Rules。
*   **Glob Pattern**: 根據檔案路徑模式（例如 `src/**/*.ts`）自動套用。

---
導覽：[<- Settings](settings.md) | [Workflows ->](workflows.md)

---

> **原文參考**：[antigravity.google/docs/rules-workflows](https://antigravity.google/docs/rules-workflows)
