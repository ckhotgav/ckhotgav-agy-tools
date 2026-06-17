# ckhotgav-agy-tools 專案開發進度表

本檔案記錄本工具箱（AGY2 專用版）的開發與維護進度，同時做為學生學習「如何使用 PROJECT.md 管理專案」的範本。

---

## 🎯 目前開發進度
- [x] 已完成：README.md 與主文件規劃
- [/] 進行中：技能 00 至 20 完整結構與內容
- [ ] 待處理：全域開工 (startup) 與收工 (shutdown) 技能優化
- [ ] 待處理：自動化寫入 `mcp_config.json` 機制測試
- [ ] 待處理：系統健康檢查與 doctor 技能測試

---

## 📝 開發里程碑與技術細節
* **2026-06-18 重構核心機制**：
  * 修改了 Obsidian (11) 與 NotebookLM (02) 的 MCP 設定語法，改為寫入 `mcpServers` 的 AGY2 相容 JSON 物件。
  * 將圖片生成技能 (10) 重新設計，改為以 Gemini 的生圖模型 Imagen 3 (nanobanana) 為主引導，發揮文字渲染與高保真特色。
  * 優化了全域專案助理的開工/收工，使其自動檢查並讀寫專案目錄的 `PROJECT.md` 與 Obsidian 的每日筆記。
