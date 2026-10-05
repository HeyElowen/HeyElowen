# HeyElowen / Elowen

**3D WebGIS** · Java / Vue / Cesium / PostGIS

[中文](https://github.com/HeyElowen/HeyElowen/blob/main/README.md) · [English](https://github.com/HeyElowen/HeyElowen/blob/main/README.en.md) · [繁體中文](https://github.com/HeyElowen/HeyElowen/blob/main/README.zh-TW.md) · [日本語](https://github.com/HeyElowen/HeyElowen/blob/main/README.ja.md) · **한국어** · [Español](https://github.com/HeyElowen/HeyElowen/blob/main/README.es.md) · [Français](https://github.com/HeyElowen/HeyElowen/blob/main/README.fr.md)

---

"돌로 갈아야, 무딘 것이 날카로워진다."(石以砥焉，方能化鈍為利)

저는 지리정보과학을 전공하고 3D WebGIS를 만듭니다. 무딘 쇠가 날카로운 칼이 되려면 먼저 돌에 갈려야 합니다 — 저는 이 문장을 프로젝트를 고르는 방식으로 삼습니다. 하기 쉬운 것이 아니라, 정말로 저를 갈아 주는 것을 고릅니다.

최근에 갈아 낸 것은 「碳语智图」: 공간 분석 도구를 스스로 편성하고, 우시대학(無錫學院) 주변 800m의 탄소 배출량을 조사해 그 결론을 보고서로 정리하는 AI 에이전트입니다. Cesium 3D 씬 위에서 동작합니다.

---

## 지금 하는 일

### 碳语智图 · 도시 탄소 배출량 3D 시각 분석 시스템

"우시대학 주변 800m의 탄소 배출 현황을 조사하라"는 한 마디 지시만으로 시스템이 스스로 움직입니다: 스킬 로드 → 도구 편성 → 버퍼·중첩 분석 → 3D 씬에서 배출량에 따라 단계적으로 하이라이트 → 도표가 포함된 보고서 출력.

백엔드는 LLM을 '두뇌'로, 등록된 8개의 도구를 '손발'로 삼는 공간 분석 에이전트로, '진입 → 편성 → 엔진 → 도구' 4계층으로 나뉘어 있으며 각 계층의 책임은 단일하고 의존은 단방향입니다. 프런트엔드는 SSE로 에이전트의 실행 과정을 실시간으로 받아 각 단계를 Cesium 3D 씬에 재현합니다.

프런트엔드 [`twin-carbon-web`](https://github.com/HeyElowen/twin-carbon-web) · 백엔드 [`twin-carbon-boot`](https://github.com/HeyElowen/twin-carbon-boot)

---

## 기술 스택

| 분야 | 기술 |
| --- | --- |
| 공간 | PostGIS · Cesium · SuperMap iClient 3D · 버퍼 / 중첩 분석 |
| 백엔드 | Java 17 · Spring Boot 4 · MyBatis · SSE |
| 프런트엔드 | Vue 3 · Vite · Element Plus · ECharts |
| AI | DeepSeek Function Calling · 도구 편성 |

---

## 연락처

- 이메일 · 3293400882@qq.com
- GitHub · [github.com/HeyElowen](https://github.com/HeyElowen)

---

우시대학 · 지리정보과학 · 2027년 졸업 예정 · WebGIS / 공간 데이터 분야 인턴십 및 신입 채용을 찾고 있습니다
