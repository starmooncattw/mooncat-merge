# 🐱 星月貓滑倒遊戲

基於 [moonfloof/suika-game](https://github.com/moonfloof/suika-game) 修改的星月貓滑倒遊戲，使用 Matter.js 物理引擎打造。

> 專案起源：看到 [這則貼文](https://x.com/i/status/2066760278558302679) 產生的後續創作

## ✨ 特色

- **8 個貓咪等級**：喵 → 總 → 宇 → 宙 → 天 → 下 → 無 → 敵
- **響應式設計**：支援電腦與手機遊玩
- **自訂角色圖片**：可愛貓咪取代水果
- **底部狀態列**：顯示最高分、下一個貓咪、重新開始按鈕
- **手機版優化**：
  - 右上角「📋 等級」按鈕可查看貓咪階級
  - 使用 `100dvh` 避免瀏覽器功能列遮擋
  - 彈出式等級視窗

## 🎮 遊戲玩法

1. 點擊螢幕放下貓咪
2. 兩隻相同的貓咪碰撞會合體升級
3. 不要讓貓咪堆疊超過頂部紅線
4. 挑戰合成最終形態「敵」！

## 🛠️ 技術架構

- **純前端**：HTML + JavaScript
- **物理引擎**：[Matter.js](https://brm.io/matter-js/)
- **響應式設計**：CSS Media Query（@media max-width: 768px）
- **部署方式**：GitHub Pages

## 📁 專案結構

```
mooncat-merge/
├── index.html           # 遊戲主頁面
├── index.js             # 遊戲邏輯
├── matter.js            # 物理引擎
└── assets/
    ├── img/
    │   ├── circle0.png  # 喵（等級 1）
    │   ├── circle1.png  # 總（等級 2）
    │   ├── ...
    │   └── circle7.png  # 敵（等級 8）
    ├── bg-menu.png      # 首頁背景
    └── btn-start.png    # 開始按鈕
```

## 🎨 素材來源

| 項目 | 來源 | 授權 |
|------|------|------|
| 遊戲引擎 | [moonfloof/suika-game](https://github.com/moonfloof/suika-game) | Unlicense（公共領域） |
| 角色圖片 | [@Inami0905](https://x.com/Inami0905) - [貼文](https://x.com/Inami0905/status/2068997428619972931) | 已獲繪師同意 |

## 🚀 本機執行

```bash
# Clone 專案
git clone https://github.com/starmooncattw/mooncat-merge.git
cd mooncat-merge

# 用瀏覽器開啟或啟動簡易伺服器
npx live-server
```

## 📱 響應式設計說明

### 電腦版（>768px）
- 右側顯示完整貓咪等級列表
- 底部固定狀態列

### 手機版（≤768px）
- 隱藏右側列表
- 右上角「📋 等級」懸浮按鈕
- 點擊彈出等級視窗（可點背景或 X 關閉）
- 遊戲畫面垂直置中
- 使用 `100dvh` 避免手機瀏覽器底部功能列遮擋

## 📝 Credit

- 遊戲引擎：[moonfloof/suika-game](https://github.com/moonfloof/suika-game) (Unlicense)
- 角色圖片：[@Inami0905](https://x.com/Inami0905) 授權使用
- 開發者：[@starmooncattw](https://github.com/starmooncattw)

## 📄 授權

基於原專案 Unlicense 授權，本專案同樣採用 Unlicense 發布至公共領域。
