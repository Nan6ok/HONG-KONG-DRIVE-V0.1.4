# 香港極速駕駛 V0.1.4 — 全新 Repo

## 內容
- 自製 WebGL 3D 渲染，不依賴 Google Earth、香港政府 3D 建築、Three.js 或外部 3D CDN。
- 程序化城市樓宇、道路、窗戶細節、玩家車及 AI 車流。
- 五個香港場景風格：中環金鐘、尖沙咀旺角、銅鑼灣灣仔、沙田新界、維港海旁。
- iPhone 觸控、鍵盤、追尾鏡頭、暫停、省電／平衡／高畫質設定。
- PWA manifest、Service Worker 離線快取。

## 誠實的版本範圍
這是可玩的原創 3D 城市駕駛原型。地區選項代表場景風格，並非精確地理道路拓撲或逐棟真實建築重建。交通為遊戲 AI 模擬，不是即時真實交通。汽車是程序化遊戲模型，不是工業級掃描模型。後續版本可加入有授權的道路網資料、交通燈、路口轉向及即時交通 API。

## 建立新 GitHub Repo
1. GitHub → New repository。
2. 名稱輸入 `hong-kong-drive-v014`，建議 Public。
3. 建立後進入 Repo → Add file → Upload files。
4. 解壓 ZIP，把五個檔案（index.html、manifest.webmanifest、sw.js、icon.svg、README.md）全部上載至根目錄。
5. Commit changes。
6. Settings → Pages → Build and deployment → Deploy from a branch。
7. Branch 選 `main`，Folder 選 `/ (root)`，Save。
8. 等待 Actions 的 Pages build and deployment 顯示綠色成功。
9. 開啟 `https://你的GitHub帳號.github.io/hong-kong-drive-v014/`。

## iPhone 測試
使用 Safari 一般瀏覽模式先測試，建議先選「省電」畫質。私密瀏覽可能不保留 Service Worker 快取，不適合作離線測試。遊戲第一次開啟後按「開始駕駛」。

## 控制
左／右轉向；油門加速；煞車減速；鏡頭切換視角；Ⅱ 暫停；⚙ 選擇區域與畫質。
