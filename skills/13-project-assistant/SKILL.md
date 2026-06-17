---
name: 13-project-assistant
description: 專案助理安裝 — 部署 startup / shutdown 全域技能到編輯器技能目錄。
---

# 技能 13：專案助理部署

部署全域的 `startup`（開工）與 `shutdown`（收工）技能。

## 步驟 1：詢問你的設定偏好
AI 助理會問你三個簡單的問題：
1. 你的 Obsidian Vault 路徑（例如 `D:\Obsidian`）。
2. 每日日記儲存資料夾（預設 `每日筆記`）。
3. AI 的回覆語言（預設 `繁體中文`）。

## 步驟 2：自動寫入全域技能目錄
* AI 助理會取得當前系統的 AGY2 技能目錄：`C:\Users\user\.gemini\antigravity\skills/`。
* AI 助理會建立 `skills/startup` 與 `skills/shutdown` 目錄。
* 自動將帶入變數的新版 `startup/SKILL.md` 與 `shutdown/SKILL.md` 寫入。

## 步驟 3：重新啟動編輯器
重啟後，不論在哪個專案，你只要對 AI 說「開工」、「收工」，AI 就會自動執行進度讀取與工作記錄！
