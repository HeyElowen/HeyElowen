# HeyElowen / Elowen

**三維 WebGIS** · Java / Vue / Cesium / PostGIS

[中文](https://github.com/HeyElowen/HeyElowen/blob/main/README.md) · [English](https://github.com/HeyElowen/HeyElowen/blob/main/README.en.md) · **繁體中文** · [日本語](https://github.com/HeyElowen/HeyElowen/blob/main/README.ja.md) · [한국어](https://github.com/HeyElowen/HeyElowen/blob/main/README.ko.md) · [Español](https://github.com/HeyElowen/HeyElowen/blob/main/README.es.md) · [Français](https://github.com/HeyElowen/HeyElowen/blob/main/README.fr.md)

---

石以砥焉，方能化鈍為利。

我讀地理資訊科學，寫三維 WebGIS。一塊鈍鐵要成利器，得先在石頭上磨 —— 我把這句話當成做專案的方式：不挑好上手的，挑真的能把我磨快的。

最近磨出來的是「碳語智圖」：一個能自己調度空間分析工具、查完無錫學院周邊 800 公尺的碳排放、再把結論寫成報告的 AI Agent，跑在 Cesium 的三維場景裡。

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
