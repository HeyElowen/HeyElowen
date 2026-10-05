# HeyElowen / Elowen

**三维 WebGIS** · Java / Vue / Cesium / PostGIS

**中文** · [English](https://github.com/HeyElowen/HeyElowen/blob/main/README.en.md) · [繁體中文](https://github.com/HeyElowen/HeyElowen/blob/main/README.zh-TW.md) · [日本語](https://github.com/HeyElowen/HeyElowen/blob/main/README.ja.md) · [한국어](https://github.com/HeyElowen/HeyElowen/blob/main/README.ko.md) · [Español](https://github.com/HeyElowen/HeyElowen/blob/main/README.es.md) · [Français](https://github.com/HeyElowen/HeyElowen/blob/main/README.fr.md)

---

石以砥焉，方能化钝为利。

我读地理信息科学，写三维 WebGIS。一块钝铁要成利器，得先在石头上磨 —— 我把这句话当成做项目的方式：不挑好上手的，挑真的能把我磨快的。

最近磨出来的是「碳语智图」：一个能自己调度空间分析工具、查完无锡学院周边 800 米的碳排放、再把结论写成报告的 AI Agent，跑在 Cesium 的三维场景里。

---

## 在做什么

### 碳语智图 · 城市碳排放三维可视分析系统

一句指令「调查无锡学院周边 800m 的碳排放情况」，系统自己动起来：加载技能 → 编排工具 → 缓冲区叠加分析 → 三维场景里按排放高低分级高亮 → 输出图文报告。

后端是一个以 LLM 为大脑、8 个注册工具为手脚的空间分析 Agent，按「入口 → 编排 → 引擎 → 工具」四层拆开，各层职责单一、依赖单向；前端用 SSE 实时接收 Agent 的执行过程，把每一步搬进 Cesium 的三维场景。

前端 [`twin-carbon-web`](https://github.com/HeyElowen/twin-carbon-web) · 后端 [`twin-carbon-boot`](https://github.com/HeyElowen/twin-carbon-boot)

---

## 技术栈

| 方向 | 技术 |
| --- | --- |
| 空间 | PostGIS · Cesium · SuperMap iClient 3D · 缓冲区 / 叠加分析 |
| 后端 | Java 17 · Spring Boot 4 · MyBatis · SSE |
| 前端 | Vue 3 · Vite · Element Plus · ECharts |
| AI | DeepSeek Function Calling · 工具编排 |

---

## 联系

- 邮箱 · 3293400882@qq.com
- GitHub · [github.com/HeyElowen](https://github.com/HeyElowen)

---

无锡学院 · 地理信息科学 · 2027 届 · 正在寻找 WebGIS / 空间数据方向的实习与校招机会
