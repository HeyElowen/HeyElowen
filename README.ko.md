# HeyElowen / Elowen

**3D WebGIS** · Java / Vue / Cesium / PostGIS

[中文](https://github.com/HeyElowen/HeyElowen/blob/main/README.md) · [English](https://github.com/HeyElowen/HeyElowen/blob/main/README.en.md) · [繁體中文](https://github.com/HeyElowen/HeyElowen/blob/main/README.zh-TW.md) · [日本語](https://github.com/HeyElowen/HeyElowen/blob/main/README.ja.md) · **한국어** · [Español](https://github.com/HeyElowen/HeyElowen/blob/main/README.es.md) · [Français](https://github.com/HeyElowen/HeyElowen/blob/main/README.fr.md)

---

지리정보과학을 전공하고 3D WebGIS를 축으로 공부하고 있습니다. 제 학습 방식은 대체로 "문제가 생긴 뒤에 도구를 찾는" 쪽입니다. 공간 데이터를 다뤄야 하면 PostGIS를, 도시를 브라우저에 올리고 싶으면 Cesium을, 분석 흐름을 스스로 돌리고 싶으면 에이전트가 도구를 어떻게 편성하는지를 파고듭니다. 지금 만드는 것들은 그렇게 조금씩 자라났습니다.

*"돌로 갈아야, 무딘 것이 날카로워진다." — 石以砥焉，方能化鈍為利*

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
