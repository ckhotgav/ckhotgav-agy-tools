# ckhotgav-agy-tools 點哥AI全能工具箱 (AGY2 專用版)

AI 編輯器 (**AntiGravity 2**) 新手全能懶人包。幫助完全不懂程式的新手快速建立 AI 開發與知識管理環境。

---

## 🎯 這個工具箱能幫你做什麼？
本工具箱包含 21 項獨立模組化技能，支援：
* **環境自動配置**：自動安裝 Node.js、Python、Git 等開發底座。
* **網頁一鍵發布**：寫好網頁後，由 AI 自動呼叫 Netlify / FTP 部署上網。
* **雲端與本地資料庫**：連線 Supabase、Firebase 以及 MySQL。
* **雙腦知識庫管理**：本地 Obsidian 筆記庫與雲端 Google NotebookLM 的無縫整合與 MCP 連結。
* **自動專案助理（開工/收工）**：全自動進度總結、日誌更新，且部署與否完全由你決定。
* **AI 繪圖引導**：教你如何善用 Gemini / nanobanana (Imagen 3) 生圖模型，將文字精準畫入圖中。

---

## 🚀 新手快速安裝指南
如果你正在使用 **AntiGravity 2**，只需將以下這行話複製並發送給 AI 助理：

```text
這是點哥AI全能工具箱（AGY2專用版）https://github.com/ckhotgav/ckhotgav-agy-tools
請讀取 repo 內容，列出所有可用的技能，問我要安裝哪些，然後自動幫我安裝。
```

AI 助理會自動讀取目錄，詢問你要安裝哪些階段的技能，並為你自動設定。

---

## 🔄 舊版 `ckhotgav-tools` 使用者無痛升級指南
如果你之前已經在舊的編輯器或舊版工具箱上安裝過技能，升級到 AGY2 極其簡單：

1. **直接覆蓋**：直接在 AGY2 中輸入上述安裝指令。
2. **全域助理覆蓋**：安裝 **技能 13**（專案助理）後，AI 會自動將新版針對 `PROJECT.md` 優化的 `startup` 與 `shutdown` 技能寫入 `C:\Users\user\.gemini\antigravity\skills/`，自動覆蓋舊版。
3. **MCP 格式修復**：新版在設定 NotebookLM (技能 02) 與 Obsidian (技能 11) 時，會**自動修正**你的 `mcp_config.json` 設定檔，將舊版的 `"mcp"` 格式轉換為 AGY2 專用的 `"mcpServers"` 格式，解決連線失效的問題。

---

## 📂 學習資源
* 完整詳細說明：請參考 [點哥AI全能工具箱.md](file:///d:/ANTI%20%E8%AA%B2%E7%A8%8BAI%E6%95%B4%E7%90%86%E5%8D%80/AGY-2/ckhotgav-agy-tools/%E9%BB%9E%E5%93%A5AI%E5%85%A8%E8%83%BD%E5%B7%A5%E5%85%B7%E7%AE%B1.md) 或 [GUIDE.md](file:///d:/ANTI%20%E8%AA%B2%E7%A8%8BAI%E6%95%B4%E7%90%86%E5%8D%80/AGY-2/ckhotgav-agy-tools/GUIDE.md)。
* 本日開發記錄：請參考 [PROJECT.md](file:///d:/ANTI%20%E8%AA%B2%E7%A8%8BAI%E6%95%B4%E7%90%86%E5%8D%80/AGY-2/ckhotgav-agy-tools/PROJECT.md)。

---

## 👨‍💻 關於作者
**點哥（昇鴻）** — 哲學與生命教育背景的程式設計教師、正念催眠培訓師。相信「程式是表達思想的工具」，致力於讓完全不會寫程式的人也能透過 AI 實現自己的想法。
* GitHub: https://github.com/ckhotgav
* Facebook: https://facebook.com/jshpapa
* Email: thinkclue@gmail.com
* 授權條款：MIT License
