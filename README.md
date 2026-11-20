# 心晴校園 Mood Campus（前端示範）

## 使用
1. 解壓縮。
2. 直接開啟 `index.html`，或用 VS Code 的 Live Server。
3. 學生頁可記錄 emoji 心情、查看 30 日平均、開啟呼吸練習及模擬 EEG 連接。
4. 老師／社工頁可切換班別，查看班級平均和轉介提示。

## 發佈到 GitHub Pages
1. 在 GitHub 建立 `mood-campus-app` repository。
2. 將 `index.html`、`style.css`、`app.js` 上載到 main branch 根目錄。
3. Settings → Pages → Deploy from a branch → main → /(root)。

## 重要：這只是 prototype
- 資料只存於瀏覽器 localStorage，沒有登入、資料庫或真正的角色權限。
- 「網上輔導員」電郵必須換成學校正式聯絡渠道。
- EEG 按鈕只模擬連接。真正連接要依設備 SDK／Web Bluetooth 規格實作，而且瀏覽器支援有限。
- 不應把學生姓名、筆記或健康資料直接放進 GitHub Pages。
- 正式上線前需要：學校批准、私隱影響評估、資料最少化、加密、權限分級、審計紀錄、保留及刪除政策，以及人工危機評估流程。

## 建議規則
- 班級圖表只在有足夠回應人數時顯示，避免重新識別個人。
- 「連續 7 日 ☹️」只產生人工覆核提示，不等同診斷或自動轉介。
- 若學生表示即時傷害風險，應顯示學校緊急程序及 999，而非只靠自動化流程。
