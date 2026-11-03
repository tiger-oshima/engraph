# Engraph

**要求と成果物の接続性を、3D空間で探索するためのモデリングツール。**

Engraphは、要求がどのように具体化され、どの成果物に結びつき、何によって検証されるかを可視化する。要求管理の表や単なるタスク管理ではなく、開発の判断と成果物の構造を一体として把握することを目指す。

## ドキュメント

- [Vision — 目的と設計原則](docs/vision.md)
- [Domain Model — 概念・関係・レコード例](docs/domain-model.md)
- [3D Visualization — 表示・操作の方向性](docs/visualization.md)

## 現在の方針

- **Requirement** は目的・動機・要求・仕様・技術的制約を区別せず扱い、対象が未定でも登録できる。
- **Derivation** はRequirementからRequirementへの導出を表す。
- **Artifact** は成果物を表し、自己参照によって包含階層を持つ。SystemやDatabaseなどの種類はCoreにハードコーディングしない。
- **Realization** はRequirementと、それを実現するArtifactの対応を表す。
- **Validation** は導出の妥当性、**Verification** は実現の充足を評価する。
- 主要UIは**Three.jsによる3Dグラフ**。Artifactは黄色い立方体、Requirementは青い球体で表示する。

本リポジトリは構想・ドメインモデルの整理段階。ここに記載する設計案は実装済みであることを意味しない。
