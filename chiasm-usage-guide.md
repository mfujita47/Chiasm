---
marp: true
theme: chiasm
paginate: true
---

<!-- _class: title -->

# Chiasmテーマ使用ガイド

## Marpカスタムテーマの完全マニュアル

2026年2月4日

---

<!-- _class: subTitle -->

# 目次

## このガイドで学べること

---

<!-- _class: twoColumns -->

# Chiasmテーマとは

<div>

## 概要

<div class="box blue">

**Marp専用カスタムテーマ**

2段組みレイアウトと豊富なコンポーネントで情報密度の高いスライドを作成

</div>

- Markdown + HTML構文
- 視覚的に洗練されたデザイン
- プレゼンテーション効率を向上

</div>
<div>

## 主な特徴

1. <span class="tag main">2段組み</span> 情報密度の向上
2. <span class="tag accent">カラーボックス</span> 重要箇所の強調
3. セクション区切りで構造化
4. タグ・矢印で視線誘導

</div>

---

<!-- _class: subTitle -->

# 基本設定

## フロントマター記述

---

<!-- _class: twoColumns -->

# フロントマターの書き方

<div>

## 必須項目

```
---
marp: true
theme: chiasm
paginate: true
---
```

<div class="box yellow">

**重要**
必ずファイルの先頭に記述すること

</div>

</div>
<div>

## 各項目の意味

- **marp: true** - Marp機能を有効化
- **theme: chiasm** - Chiasmテーマを指定
- **paginate: true** - ページ番号を表示

</div>

---

<!-- _class: subTitle -->

# スライドの種類

## 3つの基本クラス

---

<!-- _class: twoColumns -->

# タイトルスライド（表紙）

<div>

## 記述方法

```
<!-- _class: title -->

# メインタイトル

## サブタイトル

発表者名 • 2026年2月4日
```

</div>
<div>

## 用途と特徴

<div class="box green">

**プレゼンテーション開始時**

- 大きなタイトル表示
- 視覚的にインパクト
- 発表者情報を記載

</div>

</div>

---

<!-- _class: twoColumns -->

# セクション区切り（中表紙）

<div>

## 記述方法

```
<!-- _class: subTitle -->

# セクションタイトル

## サブタイトル（任意）
```

</div>
<div>

## 用途と特徴

<div class="box blue">

**章の切り替え時**

- 濃いグレー背景
- トピック転換を明示
- 聴衆の注意を引く

</div>

</div>

---

<!-- _class: twoColumns -->

# 2段組みレイアウト（基本）

<div>

## 記述方法

```
<!-- _class: twoColumns -->

# スライドタイトル

<div>
左カラムの内容
</div>
<div>
右カラムの内容
</div>
```

</div>
<div>

## 用途と特徴

<div class="box red">

**最重要レイアウト**

- 情報密度を最大化
- 対比・比較表現
- 一般コンテンツに推奨

</div>

<span class="tag accent">推奨</span> 基本的にこのレイアウトを使用

</div>

---

<!-- _class: subTitle -->

# コンポーネント

## HTMLタグを活用した要素

---

<!-- _class: twoColumns -->

# 箱（強調ボックス）

<div>

## 基本構文

```
<div class="box">
基本ボックス（グレー）
</div>

<div class="box blue">
青色ボックス
</div>
```

## カラーオプション

- `blue` - 青色（定義・概念）
- `green` - 緑色（成功・推奨）
- `yellow` - 黄色（注意・警告）
- `red` - 赤色（重要・エラー）

</div>
<div>

## 実例

<div class="box blue">

**定義**
免疫チェックポイント阻害剤とは、がん細胞が免疫細胞にかけるブレーキを解除する薬剤

</div>

<div class="box green">

**推奨事項**
2段組みレイアウトの積極的活用

</div>

</div>

---

<!-- _class: twoColumns -->

# タグ（分類ラベル）

<div>

## 基本構文

```
<span class="tag main">メイン</span>
<span class="tag accent">重要</span>
```

## テーマ種類

- `main` - 青色タグ
- `accent` - 赤色タグ

</div>
<div>

## 活用例

1. <span class="tag main">基礎</span> 免疫学の基本概念
2. <span class="tag accent">重要</span> T細胞の活性化機序
3. <span class="tag main">応用</span> 臨床への適用

箇条書きの分類に便利

</div>

---

<!-- _class: twoColumns -->

# 矢印コンポーネント

<div>

## 基本構文

```
<span class="downarrow main"></span>
<span class="uparrow accent"></span>
```

## 注意点

<div class="box yellow">

**1行消費する**

文章の横に配置不可、独立した要素として機能

</div>

</div>
<div>

## 活用例

研究仮説の提示

<span class="downarrow main"></span>

実験デザインの構築

<span class="downarrow accent"></span>

データ収集と解析

</div>

---

<!-- _class: twoColumns -->

# 枠付き画像

<div>

## 基本構文

```
![border](画像URL)
```

## サイズ指定

```
![width:300px border](画像URL)
![height:200px border](画像URL)
```

</div>
<div>

## 用途

<div class="box green">

**視覚的な補強**

- スクリーンショット
- 図表・グラフ
- 写真資料

</div>

枠線により画像が際立つ

</div>

---

<!-- _class: subTitle -->

# 記述ルール

## 美しいスライドのための約束

---

<!-- _class: twoColumns -->

# 空行ルール

<div>

## 原則

<div class="box blue">

**タグ前後に空行**

`<div>` `</div>` などコンテンツの前後には必ず空行を入れる

</div>

## 悪い例

```
<div>
## 見出し
テキスト
</div>
次の内容
```

</div>
<div>

## 良い例

```

<div>

## 見出し

テキスト

</div>

次の内容
```

可読性と解析精度が向上

</div>

---

<!-- _class: twoColumns -->

# その他のルール

<div>

## 箇条書き

- シンプルで短い文言
- 1行あたり15-20語程度
- 詳細は口頭で補足

<div class="box yellow">

**注意**
長文は避け、キーワード中心に

</div>

</div>
<div>

## 数式サポート

LaTeX形式が使用可能

```
$E = mc^2$

$$
\int_0^\infty e^{-x^2} dx = \frac{\sqrt{\pi}}{2}
$$
```

インライン数式：$E = mc^2$

</div>

---

<!-- _class: twoColumns -->

# 実践例：腫瘍免疫学

<div>

## 免疫チェックポイント阻害剤

<div class="box blue">

**定義**
がん細胞が免疫細胞にかけるブレーキを解除する薬剤

</div>

主要な薬剤：
- 抗PD-1抗体
- 抗PD-L1抗体
- 抗CTLA-4抗体

</div>
<div>

## 作用機序

1. <span class="tag main">Step 1</span> T細胞の活性化
2. <span class="tag main">Step 2</span> 腫瘍認識の増強

<span class="downarrow accent"></span>

<div class="box green">

**結果**
腫瘍への免疫攻撃再開

</div>

</div>

---

<!-- _class: twoColumns -->

# ワークフロー推奨

<div>

## 作成手順

1. フロントマター設定
2. タイトルスライド作成
3. セクション構造の設計
4. 2段組みで内容展開
5. ボックス・タグで装飾

<div class="box blue">

**ポイント**
構造 → 内容 → 装飾の順

</div>

</div>
<div>

## チェックリスト

- [ ] フロントマター記述済み
- [ ] 各セクションに中表紙
- [ ] 2段組み活用
- [ ] 空行ルール遵守
- [ ] 箇条書きは簡潔
- [ ] 重要箇所にボックス

</div>

---

<!-- _class: twoColumns -->

# よくある間違い

<div>

## NG例1：空行なし

```
<div>
コンテンツ
</div>
次の内容
```

<span class="tag accent">エラー</span> レンダリング不良

## NG例2：長すぎる箇条書き

- これは非常に長い箇条書きの例で、1行に多くの情報を詰め込みすぎているため、読みにくく視覚的にも美しくありません

</div>
<div>

## OK例1：空行あり

```

<div>

コンテンツ

</div>

次の内容
```

## OK例2：簡潔な箇条書き

- シンプルで短い文言
- キーワード中心
- 口頭補足前提

</div>

---

<!-- _class: twoColumns -->

# Tips & Tricks

<div>

## レイアウトの工夫

- 左側：概念・定義
- 右側：具体例・応用

<div class="box green">

**効果的な対比**
理論と実践を同時提示

</div>

</div>
<div>

## 色の使い分け

- <span class="tag main">青</span> - 基本情報
- <span class="tag accent">赤</span> - 注意喚起

カラーボックスも同様に用途別に使い分け

</div>

---

<!-- _class: subTitle -->

# まとめ

## Chiasmテーマで効果的なプレゼンを

---

<!-- _class: twoColumns -->

# Chiasmテーマの強み

<div>

## 情報密度

<div class="box blue">

**2段組みレイアウト**
限られたスペースで最大の情報量を提供

</div>

- 対比・比較が容易
- 視線の自然な流れ
- 聴衆の理解促進

</div>
<div>

## 視覚的強調

<div class="box green">

**豊富なコンポーネント**
重要情報を効果的に際立たせる

</div>

- カラーボックス
- タグ分類
- 矢印による流れ
- 枠付き画像

</div>

---

<!-- _class: title -->

# Thank You!

## Chiasmテーマで素晴らしいプレゼンを

質問・フィードバック歓迎
