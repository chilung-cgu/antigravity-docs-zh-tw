# 工具

Antigravity 提供多種工具協助代理完成任務，包括 MCP 整合、產出物系統和知識庫。

## 工具概覽

| 工具 | 說明 |
|------|------|
| **MCP** | Model Context Protocol，擴展代理能力 |
| **產出物** | 代理工作的可驗證產出 |
| **知識庫** | 專案相關的背景資訊 |

## 代理可用工具

代理可以使用以下內建工具：

### 檔案操作
- `view_file` - 檢視檔案內容
- `write_to_file` - 創建新檔案
- `replace_file_content` - 編輯檔案

### 搜尋工具
- `grep_search` - 搜尋檔案內容
- `find_by_name` - 搜尋檔案名稱

### 終端操作
- `run_command` - 執行終端命令
- `send_command_input` - 發送輸入

### 瀏覽器操作
- `read_browser_page` - 讀取網頁
- `browser_action` - 執行瀏覽器動作

## 本章內容

- [MCP](mcp.md) - Model Context Protocol 整合
- [產出物](artifacts.md) - 任務清單、實作計畫等
- [知識庫](knowledge.md) - 專案背景資訊

---

> **提示**：代理會根據任務自動選擇適當的工具。
