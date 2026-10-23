# 理科解析：萬物的法則之眼 v3.5 檢查紀錄

- JavaScript 語法：以 `node --check assets/js/script.js` 檢查。
- ZIP 完整性：以 `unzip -t` 檢查。
- 章節頁結構：各科目獨立資料夾；每頁包含概念、重點、例題、解題思路、常見錯誤、進階挑戰、進度儲存與學科內前後頁導覽。
- 限制：本次完成靜態檔案與語法檢查，尚未以真實瀏覽器逐一點擊所有按鈕。


## v3.5 修正檢查
- `node --check assets/js/script.js`：通過。
- 已修復章節陣列漏逗號的 JavaScript 語法錯誤。
- 確認根目錄有 17 個獨立主要功能 HTML 入口頁，科目單元仍分置 `units/math`、`units/chemistry`、`units/physics`、`units/biology`、`units/earth`。
- 尚未在真實瀏覽器逐一點擊測試全部互動。


## v3.5 資料夾整理
- 已移除根目錄重複的舊版頁面與舊版樣式／腳本。
- 共用資源位於 `assets/css/`、`assets/js/`；主要頁面位於 `pages/`；章節位於 `units/`。
- 本次會再次執行 JavaScript 語法、HTML 本機連結與 ZIP 完整性檢查。


## v3.5 深色模式可讀性檢查
- 全站共用 CSS 新增深色模式對比度規則，涵蓋物理公式編號 01–04、公式選取狀態、公式展示、分類標籤、提示／結果區塊、章節頁標籤與輸入提示文字。
- 掃描 122 個 HTML 頁面：未發現使用 inline `color`／`background` 固定前景背景色的元素；色彩樣式集中於 `assets/css/style.css`。
- `node --check assets/js/script.js`：通過。
- 本機 HTML 連結檢查與 ZIP 完整性檢查於打包後執行。
- 限制：無法完成整站逐頁的真實瀏覽器互動驗收；曾嘗試 headless Chromium 截圖但程序逾時，因此不將視覺測試標示為通過。


## v3.6 探究與實作追加
- 新增 4 個獨立實驗頁面與研究院入口。
- 物理紙帶數據可產生、計算線性回歸斜率、顯示圖表並匯出 CSV。
- 化學、生物、地科頁面支援參數調整、比較組、結論與本機儲存。
- 對新增 HTML 本機連結與 JS 語法執行靜態檢查。
- 模擬結果是簡化教學模型，仍需教師引導並與實測數據區分。
