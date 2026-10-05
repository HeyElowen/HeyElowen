# HeyElowen / Elowen

**WebGIS 3D** · Java / Vue / Cesium / PostGIS

[中文](https://github.com/HeyElowen/HeyElowen/blob/main/README.md) · [English](https://github.com/HeyElowen/HeyElowen/blob/main/README.en.md) · [繁體中文](https://github.com/HeyElowen/HeyElowen/blob/main/README.zh-TW.md) · [日本語](https://github.com/HeyElowen/HeyElowen/blob/main/README.ja.md) · [한국어](https://github.com/HeyElowen/HeyElowen/blob/main/README.ko.md) · [Español](https://github.com/HeyElowen/HeyElowen/blob/main/README.es.md) · **Français**

---

J'étudie les sciences de l'information géographique, avec un axe WebGIS 3D. Ma façon d'apprendre, c'est plutôt « chercher l'outil une fois le problème posé » : pour traiter des données spatiales, je me suis plongé dans PostGIS ; pour mettre une ville dans le navigateur, j'ai appris Cesium ; pour que la chaîne d'analyse tourne toute seule, j'ai étudié comment un agent orchestre ses outils. Ce que je construis aujourd'hui a poussé comme ça, petit à petit.

*C'est à la pierre qu'on affûte : ce qui est émoussé devient tranchant.*

---

## Ce que je construis

### 碳语智图 · Analyse visuelle 3D des émissions de carbone urbaines

Une seule instruction — « étudie les émissions de carbone dans un rayon de 800 m autour de l'université de Wuxi » — et le système s'exécute seul : chargement de la compétence → orchestration des outils → analyse par buffer et superposition → mise en évidence par niveaux d'émission dans la scène 3D → génération d'un rapport illustré.

Le backend est un agent d'analyse spatiale ayant un LLM pour cerveau et 8 outils enregistrés pour mains, découpé en quatre couches (entrée → orchestration → moteur → outils), chacune à responsabilité unique et à dépendances unidirectionnelles. Le frontend reçoit en SSE le déroulé d'exécution de l'agent et rejoue chaque étape dans une scène 3D Cesium.

Frontend [`twin-carbon-web`](https://github.com/HeyElowen/twin-carbon-web) · Backend [`twin-carbon-boot`](https://github.com/HeyElowen/twin-carbon-boot)

---

## Stack

| Domaine | Technologies |
| --- | --- |
| Spatial | PostGIS · Cesium · SuperMap iClient 3D · analyse buffer / superposition |
| Backend | Java 17 · Spring Boot 4 · MyBatis · SSE |
| Frontend | Vue 3 · Vite · Element Plus · ECharts |
| IA | DeepSeek Function Calling · orchestration d'outils |

---

## Contact

- E-mail · 3293400882@qq.com
- GitHub · [github.com/HeyElowen](https://github.com/HeyElowen)

---

Université de Wuxi · Sciences de l'information géographique · Promotion 2027 · À la recherche de stages et de postes de jeune diplômé en WebGIS / données spatiales
