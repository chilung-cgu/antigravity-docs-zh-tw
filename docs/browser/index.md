# 瀏覽器概述 (Browser Overview)

Antigravity 具備開啟、讀取與控制 Chrome 瀏覽器的能力，讓您能夠測試開發中的網站、讀取網路數據源，並自動化各種瀏覽器任務。

## 運作機制

*   **子代理控制**：Antigravity 透過「子代理 (Subagent)」在瀏覽器中執行動作。
*   **視覺化紀錄**：子代理會紀錄其操作，並產生截圖與影片作為產出物 (Artifacts)。
*   **環境隔離**：為了確保安全，Antigravity 會在獨立的「瀏覽器設定檔 (Browser Profile)」中執行，不會與您的日常瀏覽歷史、Cookie 或登入資訊連結。

## 相關設定

*   **Chrome 二進位路徑 (Chrome Binary Path)**：Chrome 可執行檔的路徑。留空則自動偵測。
*   **Chrome 設定檔路徑 (Chrome Profile Path)**：特定資料夾路徑。留空則使用預設隔離路徑。

---
導覽：[<- 常見問題](../faq/index.md) | [Chrome 擴充功能 ->](chrome-extension.md)

---

> **原文參考**：[antigravity.google/docs/browser](https://antigravity.google/docs/browser)
