# Browser Overview (瀏覽器概述)

Antigravity 具備開啟、讀取與控制 Chrome Browser 的能力，讓您能夠測試開發中的網站、讀取網路數據源，並自動化各種 Browser 任務。

## Mechanism (運作機制)

*   **Subagent Control**: Antigravity 透過「Subagent」在 Browser 中執行動作。
*   **Visual Recording**: Subagent 會紀錄其操作，並產生 Screenshots 與 Videos 作為 Artifacts。
*   **Environment Isolation**: 為了確保安全，Antigravity 會在獨立的「Browser Profile」中執行，不會與您的日常瀏覽歷史、Cookie 或登入資訊連結。

## Settings (相關設定)

*   **Chrome Binary Path**: Chrome 可執行檔的路徑。留空則自動偵測。
*   **Chrome Profile Path**: 特定資料夾路徑。留空則使用預設隔離路徑。

---
導覽：[<- FAQ](../faq/index.md) | [Chrome Extension ->](chrome-extension.md)

---

> **原文參考**：[antigravity.google/docs/browser](https://antigravity.google/docs/browser)
