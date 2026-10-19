# futrdcu

《受詛咒的王城》：單頁文字探索遊戲，入口為 `index.html`。

## 啟動

需要 Python 3，不需要安裝第三方套件或執行建置。

```bash
cd /workspace/futrdcu
python3 -m http.server 8000 --bind 0.0.0.0
```

在瀏覽器開啟伺服器的 8000 埠即可遊玩。按 `Ctrl+C` 停止伺服器。
本機下載專案後，請改為先切換到自己的專案目錄。

## 遊戲與存檔

點擊「開始探索」進入遊戲；首次取得武器或進入賜福時會顯示教學。
存檔使用瀏覽器的 localStorage，不同瀏覽器或網站來源不共用存檔。

## 場景圖片

以下圖片尚未提供，可稍後放入對應路徑：

- `images/grace.jpg`
- `images/beast.png`

缺少圖片時會顯示提示，文字探索仍可進行。

## GitHub Pages 發布

在 GitHub 專案中依序開啟 **Settings → Pages**：

1. 在 **Build and deployment** 的 **Source** 選擇 **Deploy from a branch**。
2. 在 **Branch** 選擇 **main**，資料夾選擇 **/(root)**，按 **Save**。
3. 到 **Actions** 確認 Pages 部署成功，回到 **Settings → Pages** 按 **Visit site**。

預期遊戲網址為 https://113103015.github.io/futrdcu/ ，以 GitHub 實際顯示的網址為準。
首次部署可能需要數分鐘；成功後即可用手機瀏覽器開啟。
後續更新推送到 `main` 後會自動重新部署。

若修改經由 Pull Request 提交，先將 Pull Request 合併至 `main` 再等待部署。
若看不到 Pages 的分支發布選項，請確認自己的專案管理權限，以及帳號方案是否支援該儲存庫的可見性。
