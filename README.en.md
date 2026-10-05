# HeyElowen / Elowen

**3D WebGIS** · Java / Vue / Cesium / PostGIS

[中文](https://github.com/HeyElowen/HeyElowen/blob/main/README.md) · **English** · [繁體中文](https://github.com/HeyElowen/HeyElowen/blob/main/README.zh-TW.md) · [日本語](https://github.com/HeyElowen/HeyElowen/blob/main/README.ja.md) · [한국어](https://github.com/HeyElowen/HeyElowen/blob/main/README.ko.md) · [Español](https://github.com/HeyElowen/HeyElowen/blob/main/README.es.md) · [Français](https://github.com/HeyElowen/HeyElowen/blob/main/README.fr.md)

---

*Grind against the whetstone, and the blunt becomes sharp.*

I studied Geographic Information Science and build 3D WebGIS. A dull blade only turns sharp once it has met the stone — I take that as my way of picking projects: not the easy ones, but the ones that genuinely sharpen me.

The latest thing I sharpened is「碳语智图」(*Carbon-Speech Smart Map*): an AI agent that dispatches its own spatial-analysis tools, surveys the carbon emissions within 800 m of Wuxi University, and writes the findings up as a report — all on a 3D Cesium scene.

---

## What I'm building

### 碳语智图 · 3D Visual Analytics for Urban Carbon Emissions

One instruction — "survey the carbon emissions within 800 m of Wuxi University" — and the system runs on its own: load the skill → orchestrate tools → buffer and overlay analysis → grade-and-highlight in the 3D scene by emission level → emit an illustrated report.

The backend is a spatial-analysis agent with an LLM as its brain and 8 registered tools as its hands, split into four layers (entry → orchestration → engine → tools) with single responsibilities and one-way dependencies. The frontend receives the agent's execution stream over SSE and replays every step inside a 3D Cesium scene.

Frontend [`twin-carbon-web`](https://github.com/HeyElowen/twin-carbon-web) · Backend [`twin-carbon-boot`](https://github.com/HeyElowen/twin-carbon-boot)

---

## Stack

| Area | Technologies |
| --- | --- |
| Spatial | PostGIS · Cesium · SuperMap iClient 3D · buffer / overlay analysis |
| Backend | Java 17 · Spring Boot 4 · MyBatis · SSE |
| Frontend | Vue 3 · Vite · Element Plus · ECharts |
| AI | DeepSeek Function Calling · tool orchestration |

---

## Contact

- Email · 3293400882@qq.com
- GitHub · [github.com/HeyElowen](https://github.com/HeyElowen)

---

Wuxi University · Geographic Information Science · Class of 2027 · Open to internships and campus recruiting in WebGIS / spatial data
