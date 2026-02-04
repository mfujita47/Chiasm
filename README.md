**Chiasm** は、[Jzurde](https://github.com/Jzurde) 氏の [Canyon](https://github.com/Jzurde/canyon) テーマを、[mfujita47](https://github.com/mfujita47) 好みにカスタマイズした Marp 用テーマです。情報の密度と視覚的な読みやすさを重視しています。

## ✨ 特徴

- **2段組みレイアウト**: `twoColumns` クラスにより、左右に分かれた情報密度の高いスライドを簡単に作成できます。
- **リッチなコンポーネント**:
  - **Color Boxes**: 4色（青、緑、黄、赤）の強調ボックス。
  - **Tags**: 分類や重要度を示すためのラベル。
  - **Arrows**: 流れや推論を示すための矢印。
- **洗練されたタイポグラフィ**: BIZ UDPGothic をベースとした、読みやすいフォント選定。
- **自動ページネーション**: ヘッダーとフッターにわかりやすいページ番号を表示。

## 🚀 インストール

Marp の設定（VS Code の `settings.json` など）に、以下を追加してください。

```json
"markdown.marp.themes": [
  "https://raw.githubusercontent.com/mfujita47/Chiasm/main/chiasm.css"
]
```

> [!TIP]
> **ローカル利用**: `chiasm.css` をプロジェクトのディレクトリにダウンロードして、相対パスで指定することも可能です。

## 💻 使い方

スライドの先頭（フロントマター）で `theme: chiasm` を指定します。

```markdown
---
marp: true
theme: chiasm
paginate: true
---

<!-- _class: title -->

# スライドタイトル
## サブタイトル

---

<!-- _class: twoColumns -->

# 2段組みの例

<div>
左側のコンテンツ
</div>

<div>
右側のコンテンツ
</div>
```

詳細は [使用ガイド (.md)](./chiasm-usage-guide.md) または [PDF版](./chiasm-usage-guide.pdf) を参照してください。基本的な使い方は [オリジナル (Canyon) 版](https://github.com/Jzurde/canyon/) に準拠しています。

## 🤖 AI によるスライド生成

付属の [chiasm-generation-prompt.md](https://raw.githubusercontent.com/mfujita47/Chiasm/refs/heads/main/chiasm-generation-prompt.md) を LLM（ChatGPT, Claude 等）のプロンプトとして使用することで、Chiasm テーマに最適なスライド構成を自動生成できます。

1.  `chiasm-generation-prompt.md` の内容をコピーして AI に貼り付けます。
2.  スライドにしたい内容や構成案を AI に伝えます。
3.  AI が Chiasm の 2 段組みレイアウトやコンポーネントを駆使した Markdown コードを出力します。

## 🛠️ Canyon との主な違い

- **レイアウトの最適化**: 2段組み時の余白や境界線の調整。
- **コンポーネントの追加**: 矢印（uparrow, downarrow）や、ボックススタイルの拡充。
- **デザインの微調整**: 文字サイズ、行間、コントラストの最適化による可読性の向上。

## 🧑‍💻 作者

- **mfujita47 (Mitsugu Fujita)** - [https://github.com/mfujita47](https://github.com/mfujita47)

## 📄 ライセンス

[MIT License](LICENSE)

## 📜 変更履歴

詳細は [CHANGELOG.md](CHANGELOG.md) を参照してください。
