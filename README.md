# 香港極速駕駛 V0.1.5 — iPhone Safari 診斷修正版

## 本版修正
- 將大量逐物件 WebGL 繪圖呼叫改為每幀合併提交，減少 iPhone GPU/CPU 開銷。
- 加入 JavaScript / WebGL 錯誤顯示面板；若渲染失敗，不再只留下藍色畫面。
- 加入 WebGL context lost 診斷。
- 加強觸控按鈕 pointer capture，避免手指滑出按鈕後油門狀態卡住。
- Service Worker 改為 HTML 網頁優先取網絡版本，並清除舊版 hk-drive 快取，避免一直載入舊程式。
- 保留原創程序化城市、道路、玩家車及模擬交通；不使用 Google Earth 或政府 3D 模型。

## 部署
把 ZIP 內五個檔案上載到 GitHub Pages Repo 根目錄並 Commit：
`index.html`, `manifest.webmanifest`, `sw.js`, `icon.svg`, `README.md`。
確認 GitHub Actions 的 Pages build and deployment 成功後，Safari 用一般瀏覽模式開啟網站。
如曾安裝舊版 PWA，先從主畫面移除舊捷徑，再用 Safari 重新開啟網站。

## 測試
1. 首次開啟應見開始駕駛畫面。
2. 按「開始駕駛」後應看到道路、建築物及玩家車。
3. 按住油門，速度應上升；放開後速度逐漸下降。
4. 若仍有問題，截取畫面底部紅色「遊戲診斷錯誤」訊息。

## 誠實範圍
這仍是程序化 3D 駕駛原型；香港分區為風格場景，交通為遊戲模擬，不代表真實道路精確重建或即時交通。
