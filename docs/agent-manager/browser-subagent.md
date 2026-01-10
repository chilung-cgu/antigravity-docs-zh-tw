# Browser Subagent (瀏覽器子代理)

當 Agent 需要與網頁互動時，它會調用 **Browser Subagent**。

## Technical Context (技術背景)

*   **Dedicated Model**: Subagent 運行一個專門為操作網頁優化的模型，獨立於主 Agent 模型。
*   **Tool Capabilities**: 具備點擊、捲動、輸入以及讀取 Console Logs 等能力。

## Visuals & Interaction (視覺與互動)

*   **Visual Feedback**: 啟動時，Browser 會顯示藍色邊框與顯示目前動作的小面板。為了避免衝突，此時使用者的互動會被暫時停用。
*   **Background Operation**: Subagent 可以在非聚焦的 Tab 中運行，不影響您在其他 Tabs 的工作。

## In Agent Manager (在代理管理器中的展現)

*   **Live Feed**: 提供 Subagent 進度的即時更新。
*   **Sidebar**: 顯示當前頁面的詳細資訊與 Subagent 動作。
*   **Visual Inspection**: 讓您精確看到 Agent 正在互動的網頁元素。

---
導覽：[<- Conversation View](conversation-view.md) | [FAQ ->](../faq/index.md)

---

> **原文參考**：[antigravity.google/docs/browser-subagent](https://antigravity.google/docs/browser-subagent)
