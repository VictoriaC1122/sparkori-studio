# Sparkori · 花火工作室

獨立 App 品牌官網，包含作品介紹、支援、各 App 隱私資訊及網站隱私說明。

## 本機預覽

需要 Node.js 與 Python 3，無須安裝 npm 套件。

```sh
npm run build
npm run preview
```

開啟 `http://127.0.0.1:4173/`。

## 更新內容

- `src/home.html`：首頁內容。
- `public/style.css`、`public/site.js`：整站外觀與互動。
- `data/apple-catalog.json`：App 清單與公開商店資料。
- `data/privacy-sources/`：各 App 現有政策正文與來源。
- `data/site-settings.json`：目前可用的聯絡信箱。新信箱建立並確認可收信後才替換。
- `scripts/build.mjs`：共用版型與靜態頁面產生器。

產生的 HTML 不納入版本控制。預設分支 `codex/sparkori-website` 更新時，GitHub Actions 會重新產生並部署網站；僅 `public/` 內的網站成品會發布。

## 自訂網域

購買網域後，在此專案的 Settings → Pages 設定 Custom domain，並依 GitHub 官方文件完成網域驗證及 DNS 設定。不要更動其他 App 專案或個人首頁的網域設定。

完成設定後，手動執行一次 `Publish Sparkori website`。建置流程會從 GitHub Pages 讀取網站路徑，自動支援目前的專案子路徑與未來的自訂網域根路徑。

官方說明：https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site

## 政策內容狀態

各 App 的政策正文沿用既有公開頁面，網站託管另見本站網站隱私說明。《賴瑞的調酒研究室》既有來源僅包含作品資訊網站的隱私說明，尚非完整 App 政策；頁面已標明適用範圍。

舊支援網站目前保留。購買網域並建立新聯絡信箱後，再安排政策與 App Store 連結的轉移。
