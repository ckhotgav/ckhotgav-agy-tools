---
name: ckhotgav-agy-tools
description: >
  點哥AI全能工具箱（AGY2專用版） — AI 編輯器新手全能懶人包。
  支援 Windows / macOS。
  當使用者說「點哥」「懶人包」「ckhotgav」「安裝技能」「工具箱」等關鍵字時觸發。
  觸發後請讀取此 SKILL.md 列出所有技能 (00~20)，詢問使用者要安裝哪些，
  然後按照對應的 SKILL.md 指示逐步安裝。
  注意：若使用者是 Mac，自動將 winget / PowerShell 指令轉換為 brew / zsh。
---

# 🧰 點哥AI全能工具箱 (AGY2 專用版) — 技能清單

| 編號 | 技能 | 說明 |
|------|------|------|
| `00` | 一鍵全裝 | 一次裝完所有技能 |
| `01` | 基礎環境建置 | Node.js / Python / PowerShell 設定 |
| `02` | NotebookLM 知識庫 | NBLM / 知識庫 / MCP 連接設定 |
| `03` | GitHub 版本控制 | gh / 版控 / git 設定 |
| `04` | Netlify 一鍵部署 | 靜態網頁 / 部署上線 |
| `05` | Google Apps Script | GAS / clasp 自動化設定 |
| `06` | Supabase 資料庫 | 雲端 SQL 資料庫設定 |
| `07` | Firebase 資料庫 | Google NoSQL 雲端資料庫設定 |
| `08` | Ollama 本地AI | 本機 AI 模型下載與測試 |
| `09` | Gemini 免費API | Google 免費 AI API 申請測試 |
| `10` | 生成圖片 | Gemini / nanobanana 內建生圖與引導 |
| `11` | Obsidian 本地筆記 | 筆記 / Vault / MCPVault 連接設定 |
| `12` | 知識管理系統設定引導 | 三層結構 / 模板 / 整理知識教學 |
| `13` | 專案助理 | 開工 / 收工 / 啟動專案 / 全域技能部署 |
| `14` | 系統健康檢查 | doctor / 檢查本機版本狀態 |
| `15` | 一鍵升級工具 | 升級 / update CLI 工具 |
| `16` | 疑難排解 | 報錯 / 失敗 / NPM與PIP修復 |
| `17` | 其他AI編輯器 | Claude Code / Gemini CLI / Codex CLI 說明 |
| `18` | 其他部署平台 | Vercel / Cloudflare / Railway 說明 |
| `19` | FTP 免費主機 | 架站 / ProFreeHost / 傳統資料庫設定 |
| `20` | PHP + MySQL 進階 | 動態網站 / PHP / 資料庫連線實戰 |

## 安裝流程

1. 讀取此 SKILL.md 後，以精美的 markdown 列表列出上方所有技能（分為階段一、階段二、階段三與維護工具）。
2. 詢問使用者想安裝哪些技能：
   * 可輸入「全部」或「00」
   * 可輸入多個編號，如「01, 02, 03, 04, 11, 13」
   * 可輸入組合包：
     * 「新手基礎包」（自動選擇 01, 02, 03, 04）
     * 「知識管理包」（自動選擇 11, 12, 13）
     * 「資料庫與進階包」（自動選擇 06, 07, 08, 09, 10, 19, 20）
3. 根據使用者的選擇，依序讀取對應 `skills/<編號>-<名稱>/SKILL.md`（或 `skills/` 目錄下對應編號之 SKILL.md），執行對應的安裝指令。
4. 每安裝完一項，請先向使用者回報結果，確認沒問題後再繼續下一項。

> ⚠️ **作業系統轉換提示**：若偵測到使用者的系統為 macOS，AI 助理應自動將 `winget`、`PowerShell` 等指令轉換為 `brew` 與 `zsh` 的對應版本。
