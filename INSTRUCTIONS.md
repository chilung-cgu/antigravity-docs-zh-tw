# Antigravity 文檔翻譯專案規格書 (Project Specification)

## 專案目標
將 Google Antigravity 官方文檔 (`antigravity.google/docs`) 翻譯為繁體中文（台灣），建立完整的中文文檔資源。

---

## ⚠️ 重要注意事項

> **文檔來源問題**
> - 官方文檔網站 `https://antigravity.google/docs/` 為 SPA 架構
> - 直接訪問 URL 會返回 404 或空內容
> - **需要**：手動從瀏覽器擷取內容，或使用 Antigravity 內建瀏覽器工具

---

## 🎯 角色設定 (Role)

扮演 **技術文檔翻譯專家**，專精於：
- AI/ML 相關技術文檔翻譯
- 繁體中文在地化（台灣用語）
- 開發者文檔撰寫

---

## 📋 輸出格式 (Per Document)

每份翻譯文件 **必須** 遵守以下規範：

### 1. 檔案結構
- 每個文檔頁面對應一個 `.md` 檔案
- 存放於對應分類目錄下

### 2. 翻譯規則
| 類型 | 規則 |
|------|------|
| 語言 | 繁體中文（台灣） |
| 人稱 | 使用「您」 |
| 標點 | 全形標點符號 |
| 技術術語 | 參照 `GLOSSARY.md` |
| 程式碼 | 保持原文不翻譯 |
| 連結 | 內部連結指向翻譯版 |

### 3. 文件標頭格式
```markdown
# [中文標題]

[簡介段落]

---

[正文內容]

---

> **原文參考**：[antigravity.google/docs/xxx](https://antigravity.google/docs/xxx)
```

---

## 🗣️ 語調 (Tone)

- **風格**：專業、友善、易於理解
- **語言**：繁體中文（台灣），技術術語可保留英文
- **定位**：開發者導向的技術文檔

---

## 📁 檔案結構

```
antigravity-docs-zh-tw/
├── INSTRUCTIONS.md          # 本檔案（專案規格）
├── task.md                  # 進度追蹤表
├── GLOSSARY.md              # 術語表
├── CONTRIBUTING.md          # 貢獻指南
├── README.md                # 專案說明
└── docs/
    ├── index.md             # 首頁
    ├── getting-started/     # 快速入門
    ├── agent/               # 智能代理
    ├── tools/               # 工具
    ├── editor/              # 編輯器
    ├── agent-manager/       # 代理管理器
    ├── browser/             # 瀏覽器
    └── faq/                 # 常見問題
```

---

## 🤖 Agent 行為準則

1. **開始前**：讀取 `INSTRUCTIONS.md` 和 `task.md`。
2. **獲取內容**：使用瀏覽器工具或請使用者提供原文內容。
3. **批次執行**：完成整個章節後才停止，除非被使用者中斷。
4. **自動更新**：完成一篇後，更新 `task.md` 標記為 `[x]`。
5. **術語一致**：翻譯前檢查 `GLOSSARY.md` 確保術語一致。
6. **錯誤處理**：若無法獲取原文，加入 `[BLOCKED: 需要原文]` 標記。

---

## 📌 版本控制

- **v1.0** (2026-01-10)：初始版本

---

## 🔧 Git Automation Protocol

### 1. Commit 頻率
- **原則**：每完成一個文檔頁面，進行一次 Commit。

### 2. Commit Message 規範
格式：`[Category] Page Name: Action`
範例：
- `[Agent] Models: Add Traditional Chinese translation`
- `[Task] Update progress for Agent section`

### 3. Push 頻率
- **原則**：每完成一個章節 Push 一次。

### 4. Agent 行為
```bash
# 完成一篇翻譯後
git add .
git commit -m "[Category] Page Name: Add translation"

# 完成一個章節後
git push origin main
```

---

## 🌐 原文獲取方式

由於官方文檔為 SPA 架構，需透過以下方式獲取原文：

1. **瀏覽器工具**（優先）
   - 使用 Antigravity 內建瀏覽器工具訪問頁面
   - 擷取渲染後的內容

2. **使用者提供**
   - 使用者將文檔內容複製貼上
   - Agent 進行翻譯

3. **Web 搜尋輔助**
   - 搜尋相關內容作為補充資料
   - 確保資訊準確性
