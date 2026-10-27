# 霜霜の存鑽與存歌 ❣️

使用 GitHub Pages 的靜態網站，依照 TO 存鑽與存歌網站的版面與功能調整。

- 試算表：https://docs.google.com/spreadsheets/d/1Ba5cjze8EM8bt7b1t_9vj7r3O84gJa72arwAGksP75Q/edit
- 資料：A～E 欄（存鑽老闆、存鑽數量、存歌數量、存爆數量、總數）
- 網站文字設定：L 欄放「網站標題」或「網站小標題」，相鄰 M 欄放對應文字；修改時請在 Google 試算表操作，並不是公開網頁直接寫回試算表。
- 首頁與版權頁共用 `butterfly-lavender.png`。
- 網頁載入時不先顯示舊的副標題；成功抓取資料後顯示最新讀取內容。

## 部署 GitHub Pages

解壓 ZIP 並將所有檔案（包含 `.nojekyll`）上傳至 GitHub 儲存庫根目錄。前往 Settings → Pages，選 Deploy from a branch，選 main 與 /(root)。

## 試算表權限

在 Google 試算表「共用」中將一般存取設定為「知道連結的使用者／檢視者」。網站只讀取內容，不提供編輯權限。若資料不是第一個工作表，修改 `script.js` 的 `SHEET_GID` 為該工作表網址所示 gid。

## 重要提醒

每次重新進入或整理會要求 Google 最新資料，但試算表服務端可能有快取或同步延遲；當無法成功讀取時會顯示錯誤而不假裝是最新資料。
