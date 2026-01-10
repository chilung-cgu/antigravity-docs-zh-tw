# 模型

Antigravity 支援多種 AI 模型，您可以根據任務需求選擇最適合的模型。

## 可用模型

### 推理模型

| 模型 | 說明 | 適用場景 |
|------|------|----------|
| **Gemini 3 Pro (High)** | 最強大的推理能力 | 複雜架構設計、困難除錯 |
| **Gemini 3 Pro (Low)** | 平衡效能與速度 | 一般開發任務 |
| **Gemini 3 Flash** | 快速回應 | 簡單查詢、快速編輯 |
| **Claude Sonnet 4.5** | 出色的程式碼生成 | 程式碼重構、文件撰寫 |
| **Claude Opus 4.5** | 深度分析能力 | 複雜邏輯分析 |
| **GPT-OSS** | 開源替代方案 | 基本開發任務 |

### 專用模型

除了主要推理模型，Antigravity 還使用專用模型處理特定功能：

| 功能 | 模型 |
|------|------|
| 圖片生成 | Nano Banana Pro |
| 瀏覽器操作 | Gemini 2.5 Pro UI Checkpoint |
| 上下文摘要 | Gemini 2.5 Flash |

## 切換模型

您可以透過以下方式切換模型：

1. 點擊狀態列的模型名稱
2. 從下拉選單選擇新模型
3. 或使用命令面板：`切換模型`

## 模型選擇建議

```
複雜任務 → Gemini 3 Pro (High) 或 Claude Opus 4.5
日常開發 → Gemini 3 Pro (Low) 或 Claude Sonnet 4.5
快速回答 → Gemini 3 Flash
```

## 使用配額

不同模型有不同的使用配額，請參考 [方案與定價](../faq/index.md)。

---

> **提示**：對於大型專案，建議使用 Gemini 3 Pro (High) 以獲得最佳的理解能力。
