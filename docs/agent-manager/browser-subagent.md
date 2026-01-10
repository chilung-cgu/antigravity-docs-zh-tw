# 瀏覽器子代理 (Browser Subagent)

當代理需要與網頁互動時，它會調用**瀏覽器子代理 (Browser Subagent)**。

## 技術背景

*   **專用模型**：子代理運行一個專門為操作網頁優化的模型，獨立於主代理模型。
*   **工具權限**：具備點擊、捲動、輸入以及讀取控制台日誌 (Console Logs) 等能力。

## 視覺與互動

*   **視覺回饋**：啟動時，瀏覽器會顯示藍色邊框與顯示目前動作的小面板。為了避免衝突，此時使用者的互動會被暫時停用。
*   **後台操作**：子代理可以在非聚焦的分頁中運行，不影響您在其他分頁的工作。

## 在代理管理器中的展現

*   **實況動態**：提供子代理進度的即時更新。
*   **側邊欄**：顯示當前頁面的詳細資訊與子代理動作。
*   **視覺巡檢 (Visual Inspection)**：讓您精確看到代理正在互動的網頁元素。

---
導覽：[<- 對話視圖](conversation-view.md) | [常見問題 ->](../faq/index.md)

---

> **原文參考**：[antigravity.google/docs/browser-subagent](https://antigravity.google/docs/browser-subagent)
