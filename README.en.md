# HeyElowen / Elowen

**3D WebGIS** · Java / Vue / Cesium / PostGIS

[中文](https://github.com/HeyElowen/HeyElowen/blob/main/README.md) · **English** · [繁體中文](https://github.com/HeyElowen/HeyElowen/blob/main/README.zh-TW.md) · [日本語](https://github.com/HeyElowen/HeyElowen/blob/main/README.ja.md) · [한국어](https://github.com/HeyElowen/HeyElowen/blob/main/README.ko.md) · [Español](https://github.com/HeyElowen/HeyElowen/blob/main/README.es.md) · [Français](https://github.com/HeyElowen/HeyElowen/blob/main/README.fr.md)

---

I'm studying Geographic Information Science, focused on 3D WebGIS. My way of learning is mostly "find the tool once the problem shows up": when I needed to handle spatial data, I dug into PostGIS; when I wanted to put a city in a browser, I learned Cesium; when I wanted the analysis pipeline to run itself, I looked into how an agent orchestrates its tools. Everything I build now has grown out of that, bit by bit.

*Grind against the whetstone, and the blunt becomes sharp.*

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
