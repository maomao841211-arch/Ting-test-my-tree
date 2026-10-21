# TwTrees 獨立網站

以 twtrees-master.zip 的正式 app/ 建立，保留原本介面及手機版功能。純靜態網站，免安裝套件、免建置。

## 啟用 GitHub Pages

1. 開啟本儲存庫的 **Settings → Pages**。
2. 在 **Build and deployment** 選擇 **Deploy from a branch**。
3. 選擇 **main** 分支與 **/ (root)**，按 **Save**。
4. 等待 GitHub 部署完成，再從 Pages 頁面開啟實際發布網址。

預期網址（需完成上述設定並部署成功）：
https://maomao841211-arch.github.io/Ting-test-my-tree/

## 手機使用

以 Safari 或 Chrome 開啟 HTTPS 網址，允許相機、定位與動作感測器權限。iPhone 可透過 Safari 分享選單加入主畫面。硬體功能須在真機測試。

## 獨立資料

已停用原站 Google 試算表及 MongoDB 自動上傳。資料保存在目前裝置的瀏覽器，可匯出 CSV、JSON。不同網址或不同手機的紀錄不會自動互通。請定期匯出備份。

## 本機開發

```sh
python3 -m http.server 8080 --bind 0.0.0.0
```

本機 HTTP 用於頁面開發，不提供公開網址；手機相機、GPS、感測器需要有效 HTTPS。

## 已驗證

手機尺寸 390×844 無橫向溢出、分頁切換、設定保存、JSON 匯出、離線重新載入，瀏覽器測試無 JavaScript 錯誤。公開部署與真機硬體功能須另行確認。
