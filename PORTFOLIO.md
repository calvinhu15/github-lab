# 待辦清單 Web App

這是一個在 GitHub Copilot 實戰工作坊中完成的待辦清單 Web App。專案以純前端技術實作，聚焦在待辦事項的建立、整理、完成狀態管理，以及深色模式與基本無障礙支援。

## 線上展示

https://<你的帳號>.github.io/<你的repo名稱>/

> 請將上方網址替換成實際的 GitHub Pages 網址。

## 功能

- 新增待辦事項。
- 將待辦事項標記為完成或取消完成。
- 刪除單筆待辦事項。
- 依「全部」、「未完成」或「已完成」篩選待辦事項。
- 顯示目前未完成的待辦事項數量。
- 使用瀏覽器 `localStorage` 保存待辦資料，重新整理後仍能保留內容。
- 自動依照作業系統的 `prefers-color-scheme` 偏好套用深色或淺色模式。
- 提供手動切換深色與淺色模式的按鈕。
- 批次清除所有已完成事項，並在刪除前使用確認對話框。
- 沒有已完成事項時停用「清除已完成」按鈕。
- 在篩選結果為空時顯示對應提示文字。
- 使用語意化標籤、ARIA 屬性與鍵盤可操作的原生表單控制項。
- 支援小螢幕版面配置。

## 技術

- 使用純 HTML、CSS 與原生 JavaScript。
- 不使用任何框架或第三方套件。
- 不依賴外部 CDN，可離線開啟與使用。
- 使用 CSS 變數管理主題色彩與介面狀態。
- 使用 `localStorage` 保存待辦事項資料。
- 使用 `textContent`、`createElement` 與原生 DOM API 產生清單內容。

## 開發方式

這個專案是在 GitHub Copilot 實戰工作坊中，逐步使用以下方式完成：

- **GitHub Copilot Agent Mode**：根據需求建立待辦清單的前端結構與互動功能，並協助釐清與修正 GitHub Issue。
- **MCP**：設定 Microsoft Learn 與 GitHub MCP Server，讓開發過程可以查詢官方文件並讀取 repository 的 issue。
- **Agentic workflow**：透過 `.github/prompts/fix-issue.prompt.md` 定義處理 issue 的流程，包含讀取 issue、提出修改計畫、等待確認、建立分支、修改、驗證、推送與建立 Pull Request。
- **專案規範**：使用 `.github/copilot-instructions.md` 集中記錄技術限制、程式風格與協作方式。

## 我學到什麼

- 如何使用 GitHub Copilot Agent Mode，將需求拆解成可執行的開發步驟。
- 如何透過 MCP 連接 Microsoft Learn 與 GitHub，取得較貼近開發情境的文件與 repository 資訊。
- 如何用 CSS `prefers-color-scheme` 與 CSS 變數實作深色模式。
- 如何透過 GitHub issue、分支與 Pull Request 管理一個小型功能的開發流程。
- 如何在不使用框架的情況下，使用原生 DOM API、事件處理與 `localStorage` 完成互動式 Web App。
