# 画像グリッド配置・透過クロップツール

複数画像を読み込み、列数、行数、上下左右の余白、書き出し先の画像サイズを指定してグリッド上に配置する。余白、列幅、行高はハンドルで個別調整でき、ドラッグで固定アスペクト比のクロップ範囲を作り、透過情報を保ったままPNGやWebPへ書き出す。

| 項目 | 内容 |
| --- | --- |
| Rank | 74 |
| Domain | WebApp |
| Idea No. | 12 |
| Repository | image-grid-transparent-crop-tool |
| 主な公開先 | GitHub Pages / GitHub Release |

## Implementation

- `src/product-profile.mjs`: プロダクト定義。
- `src/core.mjs`: 入力正規化とバッチ評価。
- `src/validators.mjs`: 必須項目と warning 項目の検査。
- `src/review-model.mjs`: UI/レビュー向けモデル。
- `src/report.mjs`: Markdown / HTML レポート生成。
- `src/cli.mjs`: CLI。
- `public/`: 静的WebApp。

## Validation

`npm test` で代表シナリオ、QCDS、docs ZIP、文字化け、WebApp非blank表示を検証します。

## Strict QCDS Docs

- [Remote benchmark](docs/qcds-remote-benchmark.md)
- [Strict metrics](docs/qcds-strict-metrics.json)
- [Traceability matrix](docs/traceability-matrix.md)
- [Release evidence](docs/release-evidence.json)
