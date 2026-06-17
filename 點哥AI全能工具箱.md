# 點哥 AI 全能工具箱 (AGY2 專用版)

嗨！如果你**完全不懂寫程式**，但又想指揮 AI 幫你做出超酷的網頁、自動化工具或個人知識庫，這篇指南就是為你量身打造的！

我們將使用目前最熱門的 AI 編輯器：**AntiGravity 2** (AGY2)。這款工具就像是你的「虛擬工程師」，你只要動嘴巴下指令，它就會幫你寫出複雜的程式碼並管理專案。

完整操作說明請見 [GUIDE.md](file:///d:/ANTI%20%E8%AA%B2%E7%A8%8BAI%E6%95%B4%E7%90%86%E5%8D%80/AGY-2/ckhotgav-agy-tools/GUIDE.md) 與 [README.md](file:///d:/ANTI%20%E8%AA%B2%E7%A8%8BAI%E6%95%B4%E7%90%86%E5%8D%80/AGY-2/ckhotgav-agy-tools/README.md)。

---

## 🖥️ 你是 Windows 還是 Mac？
本懶人包以 **Windows** 為主撰寫。
如果你是 **Mac** 使用者不用擔心，遇到指令時 AI 助理會自動幫你轉換成對應版本（例如將 `winget install` 換成 `brew install`）。

**快速對照表：**

| 情境 | Windows | Mac |
|------|---------|-----|
| 終端機名稱 | PowerShell | Terminal (zsh) |
| 安裝套件 | `winget install` | `brew install` |
| npm 指令 | `npm` | `npm` |
| 設定檔路徑 | `C:\Users\名字\.gemini\antigravity\mcp_config.json` | `~/.gemini/antigravity/mcp_config.json` |

---

## 🎯 我可以裝哪些技能？
這個工具箱共有 21 項技能，每一項都可以**獨立選擇要不要安裝**：

| 編號 | 技能名稱 | 難度 | 說明 |
|------|---------|:----:|------|
| **00** | 一鍵全裝 | 🟢 | 一次裝全部，省事 |
| **01** | 基礎環境建置 | 🟢 | 一定要先裝這個！安裝 Node.js 與 Python |
| **02** | NotebookLM 知識庫 | 🟢 | AI 雲端知識庫串接 (寫入 mcpServers) |
| **03** | GitHub 版本控制 | 🟢 | 程式碼的雲端時光機，防手殘 |
| **04** | Netlify 一鍵部署 | 🟢 | 把寫好的網頁放到網路上 |
| **05** | Google Apps Script | 🟡 | 雲端自動化腳本與 clasp 整合 |
| **06** | Supabase 資料庫 | 🟡 | 免費雲端 SQL 資料庫 |
| **07** | Firebase 資料庫 | 🟡 | Google 雲端 NoSQL 資料庫 |
| **08** | Ollama 本地AI | 🟡 | 在自己的電腦跑 AI，免網路 |
| **09** | Gemini 免費API | 🟡 | 申請 Google 免費 AI 密鑰測試 |
| **10** | 生成圖片 | 🟢 | **AGY2 內建 Gemini / nanobanana 生圖引導** |
| **11** | Obsidian 本地筆記 | 🟢 | 連接你的第二大腦 (寫入 mcpServers) |
| **12** | 知識管理系統設定引導 | 🟢 | 學會整理知識與建立日記範本 |
| **13** | 專案助理 | 🟢 | 開工、收工與專案初始化 (寫入全域技能) |
| **14** | 系統健康檢查 | 🟢 | 檢查本機開發環境與工具是否正常 |
| **15** | 一鍵升級工具 | 🟢 | 一鍵更新所有 CLI 工具到最新 |
| **16** | 疑難排解 | 🟢 | 常見報錯與 NPM/PIP 修復指南 |
| **17** | 其他AI編輯器 | 🟡 | 介紹 Claude Code, Codex 等工具 |
| **18** | 其他部署平台 | 🟡 | 介紹 Vercel, Cloudflare Pages 等平台 |
| **19** | FTP 免費主機 | 🟡 | 免費架站空間與 MySQL 資料庫 |
| **20** | PHP + MySQL 進階 | 🟡 | 動態網站資料庫連線 (訪客計數器) |

> 🟢 = 新手友善　🟡 = 有一點基礎再裝

---

## 🚀 新手推薦安裝順序
如果是第一次接觸，建議照這個順序來：

### 第一階段：打基礎（一定要裝）
```
00 → 01 → 02 → 03 → 04
```

### 第二階段：學會整理知識
```
11 → 12 → 13
```

### 第三階段：進階火力
```
06 → 07 → 08 → 09 → 10 → 19 → 20
```

---

## 🛠️ 部分核心技能實戰說明

### 技能 02：NotebookLM 知識庫串接
此技能將 Google 的 AI 知識庫與 AGY2 串接。
1. **安裝 CLI**：在終端機執行 `pip install notebooklm-mcp-cli`。
2. **安全登入**：在終端機手動執行 `nlm login`，完成 Google 帳號授權。
3. **自動綁定**：對著 AGY2 說「請幫我設定 NotebookLM」，AI 助理會自動在 `C:\Users\user\.gemini\antigravity\mcp_config.json` 中的 `"mcpServers"` 區塊寫入設定，不需要你手動修改 JSON 檔。

### 技能 10：Gemini / nanobanana 生成圖片
在 **AntiGravity 2** 中，生圖變得無比簡單！
* **免 API Key**：AGY2 內建了 Google 最新的 Imagen 3 引擎（即社群俗稱的 **nanobanana** 模型）。
* **如何使用**：直接對 AI 說：「幫我畫一張（你的場景描述）的圖片」。
* ** nanobanana 優勢**：這個模型極擅長在圖片中精準生成英文單字。試試看這個 prompt：「幫我畫一個賽博朋克風的霓虹燈招牌，招牌上寫著大大的 "OPEN" 字樣」，你會對結果感到驚艷！

### 技能 11：Obsidian 連結
Obsidian 是你的本地「第二大腦」。
1. **安裝外掛**：終端機執行 `npm install -g @bitbonsai/mcpvault`。
2. **路徑寫入**：將你的筆記資料夾路徑（例如 `D:\Obsidian`）告訴 AI。AI 助理會自動在 `mcp_config.json` 的 `"mcpServers"` 寫入設定。
3. **驗證**：重啟編輯器後，對著 AI 說：「幫我把這段筆記寫入 Obsidian 中」，AI 就會自動為你寫入本地資料庫。

### 技能 13：專案助理 (開工與收工)
本工具箱最靈魂的核心！
* **開工**：對 AI 說「我來了」或「開工」，AI 會讀取專案跟目錄底下的 **`PROJECT.md`** 進度表，比對暫存區，然後告訴你目前的里程碑與未完事項，**只讀不改程式碼**。
* **收工**：對 AI 說「收工」，AI 會幫你整理今天的修改、更新 `PROJECT.md`，並主動詢問你是否要進行 Git Commit、Push 或是 Netlify 部署，**所有部署均尊重你的意願**。

---

## 🎉 恭喜你完成所有安裝！
你現在已經擁有了一個由 AI 驅動的全自動開發工作站！
別害怕犯錯，有任何想法，直接對著 AI 許願就對了。需要複習時，隨時回來翻這份指南。
**Happy coding！🚀**
