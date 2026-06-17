---
name: 14-doctor
description: 系統健康檢查 — 診斷本機 Node.js、npm、Python、Git 及 CLI 版本狀態，提供自癒式修復。
---

# 技能 14：系統健康檢查

當你發現 AI 指令執行失敗時，請使用此技能。

## 使用方式
對著 AI 助理說：
> **「幫我執行系統健康檢查」** 或 **「doctor」**

AI 助理會自動檢查以下項目並列印出診斷報告：
1. **Node.js 與 NPM** 是否安裝，版本是否為 LTS。
2. **Python** 是否加入 PATH 環境變數。
3. **Git** 與 **GitHub CLI** 登入狀態是否有效。
4. **Obsidian (mcpvault)** 與 **NotebookLM** 的 MCP 設定是否正確。

若發現缺少套件，AI 助理會主動詢問你是否要由它直接代勞安裝。
