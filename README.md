# BirdsForestHub

チーム開発デモ用の GitHub Organization です。

## 現在進行中のプロジェクト

### Posture Check Demo (2026-04)

静止画から座り姿勢の良し悪しを判定するシンプルな Web アプリを、5チーム分担で開発します。

**目的**

- GitHub Organization の運用を学ぶ
- Claude Team プランの運用を学ぶ
- チーム開発のプロセス(Issue / PR / レビュー / CI / リリース)を一通り経験する

**ロードマップ**

- Phase 1 (〜 2026-04-30): 静止画での座り姿勢判定 ← **現在ここ**
- Phase 2 (2026-05 予定): 動画対応
- Phase 3 (未定): ラズパイを用いた筋トレアシスト

## チーム構成とリポジトリ

| チーム | 担当リポジトリ | 役割 |
|---|---|---|
| Andromeda | [posture-check-schema](https://github.com/BirdsForestHub/posture-check-schema) | データ構造の定義、全チームの共通基盤 |
| Camellia | [posture-check-extractor](https://github.com/BirdsForestHub/posture-check-extractor) | 画像からの姿勢抽出 |
| Dogwood | [posture-check-samples](https://github.com/BirdsForestHub/posture-check-samples) | 検証用サンプル画像の管理(Private) |
| ErigeronAnnuus | [posture-check-judge](https://github.com/BirdsForestHub/posture-check-judge) | 姿勢の良し悪し判定ロジック |
| FringedGalax | [posture-check-ui](https://github.com/BirdsForestHub/posture-check-ui) | Web UI と全体統合 |

## セキュリティ・倫理方針

このプロジェクトは以下の方針を最優先で守ります。

- 実在の第三者が写った画像は一切扱いません
- サンプル画像は Private リポジトリでのみ管理し、公開しません
- 判定結果は健康アドバイスではなく、身体的特徴によって判定が偏る可能性があることを UI 上で明示します
- 依存ライブラリのバージョンは pin し、Dependabot によって監視します
- Secret scanning と Push protection を Organization レベルで有効化しています

## ライセンス

各リポジトリの LICENSE ファイルを参照してください(原則 MIT)。
