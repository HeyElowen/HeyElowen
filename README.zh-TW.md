# HeyElowen / Elowen

**三維 WebGIS** · Java / Vue / Cesium / PostGIS

[中文](https://github.com/HeyElowen/HeyElowen/blob/main/README.md) · [English](https://github.com/HeyElowen/HeyElowen/blob/main/README.en.md) · **繁體中文** · [日本語](https://github.com/HeyElowen/HeyElowen/blob/main/README.ja.md) · [한국어](https://github.com/HeyElowen/HeyElowen/blob/main/README.ko.md) · [Español](https://github.com/HeyElowen/HeyElowen/blob/main/README.es.md) · [Français](https://github.com/HeyElowen/HeyElowen/blob/main/README.fr.md)

---

我讀地理資訊科學，方向是三維 WebGIS。我的學習路徑基本上是「遇到問題再去找工具」：需要處理空間資料，就去啃 PostGIS；想把城市搬進瀏覽器，就去學 Cesium；想讓分析流程自己跑起來，就去研究 Agent 怎麼調工具。現在做的東西，都是這麼一點點長出來的。

*石以砥焉，方能化鈍為利。*

---

## 在做什麼

### 碳語智圖 · 城市碳排放三維視覺化分析系統

一句指令「調查無錫學院周邊 800m 的碳排放情況」，系統自己動起來：載入技能 → 編排工具 → 緩衝區疊加分析 → 三維場景裡依排放高低分級高亮 → 輸出圖文報告。

後端是一個以 LLM 為大腦、8 個註冊工具為手腳的空間分析 Agent，依「入口 → 編排 → 引擎 → 工具」四層拆開，各層職責單一、依賴單向；前端用 SSE 即時接收 Agent 的執行過程，把每一步搬進 Cesium 的三維場景。

前端 [`twin-carbon-web`](https://github.com/HeyElowen/twin-carbon-web) · 後端 [`twin-carbon-boot`](https://github.com/HeyElowen/twin-carbon-boot)

---

## 技術棧

| 方向 | 技術 |
| --- | --- |
| 空間 | PostGIS · Cesium · SuperMap iClient 3D · 緩衝區 / 疊加分析 |
| 後端 | Java 17 · Spring Boot 4 · MyBatis · SSE |
| 前端 | Vue 3 · Vite · Element Plus · ECharts |
| AI | DeepSeek Function Calling · 工具編排 |

---

## 聯絡

- 電子郵件 · 3293400882@qq.com
- GitHub · [github.com/HeyElowen](https://github.com/HeyElowen)

---

無錫學院 · 地理資訊科學 · 2027 屆 · 正在尋找 WebGIS / 空間資料方向的實習與校招機會
