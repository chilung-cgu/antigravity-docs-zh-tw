# 快速入門

本指南將協助您安裝並開始使用 Google Antigravity。

## 系統需求

Antigravity 支援以下作業系統：

| 作業系統 | 版本需求 |
|----------|----------|
| **macOS** | 11.0 (Big Sur) 或更新版本 |
| **Windows** | Windows 10 (64-bit) 或更新版本 |
| **Linux** | Ubuntu 20.04 LTS 或相容發行版 |

### 硬體需求

- **記憶體**：8 GB RAM（建議 16 GB）
- **儲存空間**：2 GB 可用磁碟空間
- **網路**：穩定的網際網路連線

## 安裝步驟

### 1. 下載 Antigravity

前往 [antigravity.google/download](https://antigravity.google/download) 下載適合您作業系統的安裝程式。

### 2. 安裝應用程式

**macOS**
```bash
# 開啟下載的 .dmg 檔案
# 將 Antigravity 拖曳至應用程式資料夾
```

**Windows**
```
執行下載的 .exe 安裝程式
依照安裝精靈指示完成安裝
```

**Linux**
```bash
# Debian/Ubuntu
sudo dpkg -i antigravity_*.deb

# 或使用 AppImage
chmod +x Antigravity-*.AppImage
./Antigravity-*.AppImage
```

### 3. 首次啟動

1. 啟動 Antigravity
2. 使用 Google 帳號登入
3. 選擇偏好的 AI 模型

## 介面導覽

啟動後，您會看到三個主要區域：

```
┌─────────────────────────────────────────────┐
│  選單列                                       │
├───────────┬─────────────────────┬───────────┤
│           │                     │           │
│  檔案     │     編輯器          │  代理     │
│  總管     │                     │  側邊欄   │
│           │                     │           │
├───────────┴─────────────────────┴───────────┤
│  終端機 / 輸出                               │
└─────────────────────────────────────────────┘
```

## 第一個任務

讓我們建立一個簡單的任務來測試：

1. 在代理側邊欄輸入您的請求
2. 代理會進入「規劃」模式，產生實作計畫
3. 審核計畫後，代理會開始「執行」
4. 最後進入「驗證」模式確認結果

## 下一步

- [了解智能代理](../agent/index.md)
- [認識產出物](../tools/artifacts.md)
- [設定瀏覽器擴充功能](../browser/chrome-extension.md)

---

> **提示**：按下 `Cmd+Shift+P` (macOS) 或 `Ctrl+Shift+P` (Windows/Linux) 開啟命令面板。
