# Models (模型)

## Reasoning Model (推理模型)

對於核心 Reasoning Model (推理模型)，Antigravity 提供來自 Google Vertex Model Garden 的領先前沿模型：

- **Gemini 3 Pro (high)**
- **Gemini 3 Pro (low)**
- **Gemini 3 Flash**
- **Claude Sonnet 4.5**
- **Claude Sonnet 4.5 (thinking)**
- **Claude Opus 4.5 (thinking)**
- **GPT-OSS**

使用者可以在對話輸入框下方的 Model Selector (模型選擇器) 下拉選單中選擇要使用的 Reasoning Model：

![Model Selector](../assets/images/model-selector.png)

Reasoning Model 的選擇在單次對話的使用者訊息之間具有「黏性」(sticky)，因此如果您在 Agent 運行時更改 Reasoning Model，它將繼續使用先前選擇的 Reasoning Model，直到完成該輪使用者轉向的步驟（或直到使用者取消當前執行）。

在我們的 Plans (方案) 頁面中了解更多關於 Reasoning Model 速率限制的資訊。

## Additional Models (其他模型)

Antigravity 在技術棧的各個部分使用了一些不可自定義的其他模型：

- **Nano Banana Pro**: 當 Agent 想要生成 UI Mockup、需要圖片來填充網頁或應用程式、生成系統或架構圖以及其他生成圖像任務時，由 Generative Image Tool (生成圖像工具) 使用過。
- **Gemini 2.5 Pro UI Checkpoint**: 由 Browser Subagent (瀏覽器子代理) 使用，用於操作瀏覽器，例如點擊、滾動或填寫輸入。
- **Gemini 2.5 Flash**: 在背景中使用，用於 Checkpointing (檢查點製作) 和 Context Summarization (上下文摘要)。
- **Gemini 2.5 Flash Lite**: 由 Codebase Semantic Search Tool (程式碼庫語義搜尋工具) 使用。

---
導覽：[<- Agent](index.md) | [Modes ->](modes.md)

---

> **原文參考**：[antigravity.google/docs/models](https://antigravity.google/docs/models)
