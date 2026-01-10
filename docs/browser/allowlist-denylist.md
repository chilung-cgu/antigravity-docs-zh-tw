# Allow/Deny List (允許與拒絕清單)

Browser 使用雙層安全系統來控制網址存取。

## Core Configuration (核心配置)

### 1. Denylist (拒絕清單)
*   **Purpose**: 阻擋危險或惡意網址。
*   **Mechanism**: 使用 Google Superroots 的 BadUrlsChecker 服務。Agent 會在伺服器端進行 RPC 檢查；若伺服器無法連線，預設會拒絕存取。

### 2. Allowlist (允許清單)
*   **Purpose**: 本地端的手動清單，用於明確信任特定網址。
*   **Mechanism**: 儲存於本地文字檔中。

## Priority (優先順序)

**Denylist 始終優先。** 您無法將已出現在 Denylist 中的網址加入 Allowlist。

---
導覽：[<- Chrome Extension](chrome-extension.md) | [Chrome Profiles ->](chrome-profiles.md)

---

> **原文參考**：[antigravity.google/docs/allowlist-denylist](https://antigravity.google/docs/allowlist-denylist)
