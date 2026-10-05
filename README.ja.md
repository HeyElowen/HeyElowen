# HeyElowen / Elowen

**3D WebGIS** · Java / Vue / Cesium / PostGIS

[中文](https://github.com/HeyElowen/HeyElowen/blob/main/README.md) · [English](https://github.com/HeyElowen/HeyElowen/blob/main/README.en.md) · [繁體中文](https://github.com/HeyElowen/HeyElowen/blob/main/README.zh-TW.md) · **日本語** · [한국어](https://github.com/HeyElowen/HeyElowen/blob/main/README.ko.md) · [Español](https://github.com/HeyElowen/HeyElowen/blob/main/README.es.md) · [Français](https://github.com/HeyElowen/HeyElowen/blob/main/README.fr.md)

---

石以砥焉、方能化鈍為利。（石で研いでこそ、鈍は鋭になる。）

地理情報科学を専攻し、3D WebGIS を書いています。鈍い鉄が利器になるには、まず石で研がれなければならない —— 僕はこれを「プロジェクトの選び方」だと思っています。取り組みやすいものではなく、本当に自分を研いでくれるものを選ぶ。

最近研いだのは「碳语智图」：空間分析ツールを自分で編成し、無錫学院の周辺 800m の炭素排出量を調べ、その結論をレポートにまとめる AI エージェントです。Cesium の 3D シーン上で動きます。

---

## 今取り組んでいること

### 碳语智图 · 都市炭素排出量の 3D 可視分析システム

「無錫学院周辺 800m の炭素排出状況を調査せよ」と一言指示するだけで、システムが自ら動き出します：スキルの読み込み → ツールの編成 → バッファ・オーバーレイ分析 → 3D シーンで排出量に応じて段階的にハイライト → 図表付きレポートを出力。

バックエンドは LLM を「脳」、登録済みの 8 つのツールを「手足」とする空間分析エージェントで、「入口 → 編成 → エンジン → ツール」の 4 層に分離されており、各層の責務は単一・依存は一方向です。フロントエンドは SSE でエージェントの実行過程をリアルタイムに受け取り、その一歩一歩を Cesium の 3D シーンに再現します。

フロントエンド [`twin-carbon-web`](https://github.com/HeyElowen/twin-carbon-web) · バックエンド [`twin-carbon-boot`](https://github.com/HeyElowen/twin-carbon-boot)

---

## 技術スタック

| 分野 | 技術 |
| --- | --- |
| 空間 | PostGIS · Cesium · SuperMap iClient 3D · バッファ / オーバーレイ分析 |
| バックエンド | Java 17 · Spring Boot 4 · MyBatis · SSE |
| フロントエンド | Vue 3 · Vite · Element Plus · ECharts |
| AI | DeepSeek Function Calling · ツール編成 |

---

## 連絡先

- メール · 3293400882@qq.com
- GitHub · [github.com/HeyElowen](https://github.com/HeyElowen)

---

無錫学院 · 地理情報科学 · 2027 年卒 · WebGIS / 空間データ分野のインターン・新卒採用を探しています
