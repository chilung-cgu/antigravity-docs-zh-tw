# 設定 (Settings)

您可以透過代理的組態選項來調整其行為，包括產出物審查政策、終端機命令執行以及檔案存取權限。

## 通用設定 (Overall Settings)

### 產出物審查政策 (Artifact Review Policy)
*   **總是繼續 (Always Proceed)**：代理在產生產出物後不會詢問審查，直接繼續後續任務。
*   **請求審查 (Request Review)**：代理在執行實作計畫或關鍵產出物前，會先請求您的審查。

### 終端機命令自動執行 (Terminal Command Auto Execution)
*   **請求審查 (Request Review)**：所有終端機命令在執行前都必須經過您的核准（除了已加入「允許清單」的命令）。
*   **總是繼續 (Always Proceed)**：代理會自動執行命令，除非該命令在「拒絕清單」中。

### 代理非工作空間檔案存取 (Agent Non-Workspace File Access)
預設情況下，代理僅能存取工作空間目錄以及 `~/.antigravity/`。啟用此設定後，代理可以檢視並編輯這些邊界之外的檔案。

## 模型與內容 (Models & Context)

*   **推理模型 (Reasoning Models)**：您可以根據需要切換不同的模型（如 Gemini 3 Pro, Claude Sonnet 4.5, GPT-OSS）。
*   **黏性選擇 (Sticky Selection)**：在單一對話輪次中，您的模型選擇會保持生效直到任務完成或取消。

---
導覽：[<- 模式](modes.md) | [規則 ->](rules.md)

---

> **原文參考**：[antigravity.google/docs/agent-modes-settings](https://antigravity.google/docs/agent-modes-settings)
