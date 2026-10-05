# HeyElowen / Elowen

**WebGIS 3D** · Java / Vue / Cesium / PostGIS

[中文](https://github.com/HeyElowen/HeyElowen/blob/main/README.md) · [English](https://github.com/HeyElowen/HeyElowen/blob/main/README.en.md) · [繁體中文](https://github.com/HeyElowen/HeyElowen/blob/main/README.zh-TW.md) · [日本語](https://github.com/HeyElowen/HeyElowen/blob/main/README.ja.md) · [한국어](https://github.com/HeyElowen/HeyElowen/blob/main/README.ko.md) · **Español** · [Français](https://github.com/HeyElowen/HeyElowen/blob/main/README.fr.md)

---

Estudio Ciencias de la Información Geográfica, con foco en WebGIS 3D. Mi forma de aprender es más bien «buscar la herramienta cuando aparece el problema»: si había que tratar datos espaciales, me metí en PostGIS; si quería meter una ciudad en el navegador, aprendí Cesium; si quería que el flujo de análisis se ejecutara solo, investigué cómo un agente orquesta sus herramientas. Lo que construyo ahora ha crecido así, poco a poco.

*Con la piedra se afila: lo romo se vuelve filo.*

---

## Qué estoy construyendo

### 碳语智图 · Análisis visual 3D de emisiones de carbono urbanas

Basta una instrucción —«investiga las emisiones de carbono en 800 m alrededor de la Universidad de Wuxi»— y el sistema se pone en marcha solo: carga la habilidad → orquesta herramientas → análisis de búfer y superposición → resalta por niveles según la emisión en la escena 3D → genera un informe con gráficos.

El backend es un agente de análisis espacial con un LLM como cerebro y 8 herramientas registradas como manos, dividido en cuatro capas (entrada → orquestación → motor → herramientas), con responsabilidades únicas y dependencias en un solo sentido. El frontend recibe por SSE el proceso de ejecución del agente y reproduce cada paso dentro de una escena 3D de Cesium.

Frontend [`twin-carbon-web`](https://github.com/HeyElowen/twin-carbon-web) · Backend [`twin-carbon-boot`](https://github.com/HeyElowen/twin-carbon-boot)

---

## Stack

| Área | Tecnología |
| --- | --- |
| Espacial | PostGIS · Cesium · SuperMap iClient 3D · análisis de búfer / superposición |
| Backend | Java 17 · Spring Boot 4 · MyBatis · SSE |
| Frontend | Vue 3 · Vite · Element Plus · ECharts |
| IA | DeepSeek Function Calling · orquestación de herramientas |

---

## Contacto

- Correo · 3293400882@qq.com
- GitHub · [github.com/HeyElowen](https://github.com/HeyElowen)

---

Universidad de Wuxi · Ciencias de la Información Geográfica · Promoción 2027 · Buscando prácticas y ofertas de recién graduado en WebGIS / datos espaciales
