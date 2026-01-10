# 允許與拒絕清單 (Allow/Deny List)

瀏覽器使用雙層安全系統來控制網址存取。

## 核心配置

### 1. 拒絕清單 (Denylist)
*   **用途**：阻擋危險或惡意網址。
*   **機制**：使用 Google Superroots 的 BadUrlsChecker 服務。代理會在伺服器端進行 RPC 檢查；若伺服器無法連線，預設會拒絕存取。

### 2. 允許清單 (Allowlist)
*   **用途**：本地端的手動清單，用於明確信任特定網址。
*   **機制**：儲存於本地文字檔中。

## 優先順序

**拒絕清單始終優先。** 您無法將已出現在拒絕清單中的網址加入允許清單。

---
導覽：[<- Chrome 擴充功能](chrome-extension.md) | [Chrome 設定檔 ->](chrome-profiles.md)

---

> **原文參考**：[antigravity.google/docs/allowlist-denylist](https://antigravity.google/docs/allowlist-denylist)
