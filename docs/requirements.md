# 要件定義

| 項目 | 内容 |
| --- | --- |
| Rank | 74 |
| Domain | WebApp |
| Idea No. | 12 |
| Repository | image-grid-transparent-crop-tool |
| 主な公開先 | GitHub Pages / GitHub Release |

## 背景

画像一覧、素材シート、サムネイル、UIパーツを作る時に、グリッド配置、余白調整、固定比率クロップ、透過保持が別々の作業になりやすい。

## 目的

複数画像を読み込み、列数、行数、上下左右の余白、書き出し先の画像サイズを指定してグリッド上に配置する。余白、列幅、行高はハンドルで個別調整でき、ドラッグで固定アスペクト比のクロップ範囲を作り、透過情報を保ったままPNGやWebPへ書き出す。

## 必須要件

- grid crop job を複数件まとめて検証できる。
- required fields: `id`, `title`, `imagePath`, `gridSpec`, `cropArea`, `owner`。
- warning field: `transparentMargin`。
- 代表シナリオ、QCDS metrics、docs ZIP、release evidence を再生成できる。
