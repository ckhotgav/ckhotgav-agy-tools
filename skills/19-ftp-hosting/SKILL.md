---
name: 19-ftp-hosting
description: FTP 免費主機架站 — 申請 ProFreeHost，使用 FileZilla 上傳靜態網頁並建立 MySQL。
---

# 技能 19：FTP 免費主機架站

學習傳統的網頁架設流程，掌握 FTP 與資料庫的基本知識。

## 步驟 1：註冊 ProFreeHost
* 前往 https://profreehost.com/ 註冊，啟用帳號並點選「Create New Account」建立一個免費網域網址。

## 步驟 2：使用 FileZilla 連線
* 下載並安裝 [FileZilla Client](https://filezilla-project.org/)。
* 從 ProFreeHost 控制台取得你的 **FTP 主機 (Server)**、**FTP 帳號 (Username)** 與密碼。
* 在 FileZilla 中輸入上述資訊（Port 填寫 `21`），點選快速連線。

## 步驟 3：上傳 index.html
* 在 FileZilla 右側視窗，找到 `public_html` 資料夾。
* 將 AI 幫你寫好的網頁拖曳進該資料夾覆蓋。打開瀏覽器輸入你的網址即可看到成果！

## 步驟 4：建立 MySQL 資料庫
* 在 ProFreeHost 的 Control Panel (cPanel) 中，點選「MySQL Databases」，建立一個資料庫並記下連線帳號與密碼。
