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

### 1. 翻譯風格 (Translation Style)
- **保留專有名詞英文**：所有 Antigravity 的專有功能名稱、介面術語、技術名詞，一律**保留英文原文**，不進行翻譯。
    - 正確：Agent, Artifacts, Playground, Inbox, Workflow, Settings
    - 錯誤：智能代理, 產出物, 遊樂場, 收件匣, 工作流程, 設定
- **術語表用途**：`GLOSSARY.md` 僅作為術語的「中文解釋」參考，非翻譯對照表。
- **語氣**：使用專業、簡潔的繁體中文（台灣慣用語）。
- **標點符號**：使用全形標點符號。英文與中文之間需留有空白 (Space)。

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

1.  **開始前**：讀取 `INSTRUCTIONS.md` 和 `task.md`。
2.  **全量執行 (Batch Mode)**：
    -   **預設模式**：除非使用者明確指定單一任務，否則 Agent 應**連續執行** `task.md` 中的所有未完成項目。
    -   **不中斷**：完成一個檔案後，自動進入下一個，**不需要**每次都詢問使用者，直到遇到 [BLOCKED] 或所有任務完成。
3.  **獲取內容**：
    -   使用 Antigravity 內建瀏覽器工具訪問頁面。
    -   若遇到 SPA 載入問題，嘗試多種 selector 或等待載入。
    -   若完全無法獲取，標記 [BLOCKED] 並繼續下一頁。
4.  **自動更新**：每完成一篇，更新 `task.md` 標記為 `[x]`。
5.  **安全性檢查**：在 Commit 前，檢查檔案是否含有 PII 或敏感字串（如 `leo.wu`, `password` 等）。
6.  **術語一致**：翻譯前檢查 `GLOSSARY.md` 確保術語一致。

---

## 📌 版本控制

- **v1.1** (2026-01-10)：新增全量翻譯模式，優化 Repository 設置流程。
- **v1.0** (2026-01-10)：初始版本

---

## 🔧 Git Automation Protocol

### 1. Repository Setup
Remote Repository 已建立：`https://github.com/chilung-cgu/antigravity-docs-zh-tw`

首次推送（已完成）：
```bash
git remote add origin https://github.com/chilung-cgu/antigravity-docs-zh-tw.git
git branch -M main
git push -u origin main
```

### 2. Commit 頻率
- **原則**：每完成一個文檔頁面，進行一次 Commit。
- **指令**：
    ```bash
    git add .
    git commit -m "[Category] Page Name: Add translation"
    ```

### 3. Push 頻率
- **原則**：每完成 **3-5 個檔案** 或 **一個完整章節** 後 Push 一次，確保雲端同步但不過於頻繁。
- **指令**：
    ```bash
    git push origin main
    ```

### 4. Security & Privacy
- **嚴禁洩漏 PII**：禁止在文檔中包含任何個人密碼、金鑰、或非公開的個人資訊。
- **僅翻譯內容**：專注於文檔內容翻譯，不要將開發環境的敏感資訊寫入 `.md` 檔案。
- **偵測與攔截**：若在原文中發現敏感資訊，Agent 應自動進行去識別化處理或跳過，並通知使用者。

### 5. 錯誤處理
- 若 Push 失敗（如遇到 conflicts 或驗證問題），Agent 應暫停並通知使用者。

### 6. 部署協定 (Deployment Protocol)

為了提供更好的閱讀體驗，本專案將使用 **MkDocs** 搭配 **Material for MkDocs** 主題，並透過 **GitHub Actions** 自動部署至 GitHub Pages。

- **配置檔案**：`mkdocs.yml`
- **自動化流程**：`.github/workflows/deploy.yml` (Modern Mode)
- **部署方式**：`actions/deploy-pages` (無 `gh-pages` 分支)
- **GitHub 設定**：Pages Source 必須設定為 **GitHub Actions**。

當進行文檔結構變更時，請務必確認 `mkdocs.yml` 中的 `nav` 設定是否同步更新。

---

## 🌐 原文獲取詳情
由於官方文檔為 SPA 架構，需透過以下優先順序獲取內容：
1. **瀏覽器工具**：使用 `open_browser_url` 和 `read_browser_page` 讀取渲染後的 DOM。
2. **手動提供**：若自動化失敗，標記任務為 [BLOCKED] 並請使用者提供。

