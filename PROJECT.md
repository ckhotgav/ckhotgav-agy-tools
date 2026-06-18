# ckhotgav-agy-tools 專案開發進度表

本檔案記錄本工具箱（AGY2 專用版）的開發與維護進度，同時做為學生學習「如何使用 PROJECT.md 管理專案」的範本。

---

## 🎯 目前開發進度
- [x] 已完成：README.md 與主文件規劃
- [x] 已完成：技能 00 至 20 完整結構與內容
- [x] 已完成：全域開工 (startup) 與收工 (shutdown) 技能優化
- [x] 已完成：自動化寫入 `mcp_config.json` 機制測試
- [x] 已完成：系統健康檢查與 doctor 技能測試
- [x] 已完成：將 ckhotgav-agy-tools 公開儲存庫成功部署至 GitHub
- [x] 已完成：專案初始化 (project-init) 新增自設模板與全方位安全型 `.gitignore` 機制

---

## 📝 開發里程碑與技術細節
* **2026-06-18 專案初始化功能增強與安全性加強**：
  * 在「啟動專案」中新增了第 5 個選項「其他」，支持使用者自設語言（如 Go, Rust 等）或自定義目錄結構，並由 AI 助理動態分析並建立。
  * 加強了所有初始化專案的 `.gitignore` 安全防護規劃，預設自動屏蔽所有敏感私鑰、環境變數檔案（如 `.env*`）、金鑰檔案（`*.pem`, `*.key`）以及本地 IDE 臨時檔案。
  * 更新了 `GUIDE.md` 及 `點哥AI全能工具箱.md`，納入對於 `.gitignore` 防漏與 API Key 安全性的詳細說明與指引。
* **2026-06-18 重構與發布**：
  * 修改了 Obsidian (11) 與 NotebookLM (02) 的 MCP 設定語法，改為寫入 `mcpServers` 的 AGY2 相容 JSON 物件。
  * 將圖片生成技能 (10) 重新設計，改為以 Gemini 的生圖模型 Imagen 3 (NanoBanana) 為主引導，發揮文字渲染與高保真特色。
  * 優化了全域專案助理的開工/收工，使其自動檢查並讀寫專案目錄的 `PROJECT.md` 與 Obsidian 的每日筆記。
  * **GitHub 成功部署**：解決了信箱隱私保護阻擋，成功發布至 `https://github.com/ckhotgav/ckhotgav-agy-tools`。
  * **技能 11 實地測試**：成功為使用者的 AGY2 本地環境寫入正確的 Obsidian MCP 路徑參數 `D:\\Obsidian`。
