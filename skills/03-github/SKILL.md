---
name: 03-github
description: GitHub 版本控制 — 安裝 Git 與 GitHub CLI，登入並設定名稱及信箱。
---

# 技能 03：GitHub 版本控制

為你的程式碼提供雲端備份與還原功能。

## 步驟 1：安裝 Git
* **Windows** (AI 助理執行)：`winget install --id Git.Git -e --source winget`
* **macOS** (AI 助理執行)：`brew install git`

## 步驟 2：安裝 GitHub CLI (命令列工具)
* **Windows** (AI 助理執行)：`winget install --id GitHub.cli -e --source winget`
* **macOS** (AI 助理執行)：`brew install gh`

## 步驟 3：登入 GitHub 帳號
* 終端機執行：`gh auth login --web --git-protocol https`
* AI 助理會請使用者注意瀏覽器視窗，登入帳號並在瀏覽器輸入對話框顯示的八位數授權碼。

## 步驟 4：設定使用者資訊
* `git config --global user.name "你的英文暱稱"`
* `git config --global user.email "你的帳號@gmail.com"`
