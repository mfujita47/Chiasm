# 🎨 Chiasm - Marp Theme (v1.0.0)
**Chiasm** は、情報の密度と視覚的な洗練さを両立させた Marp 用のカスタムテーマです。
[Jzurde](https://github.com/Jzurde) 氏による [Canyon](https://github.com/Jzurde/canyon) テーマの設計思想を継承し、さらに洗練されたレイアウトとコンポーネントを追加した改良版です。

## ✨ 特徴

- 🖼️ **2段組みレイアウト**: `twoColumns` クラスにより、左右に分かれた情報密度の高いスライドを簡単に作成できます。
- 🧱 **リッチなコンポーネント**:
  - 🟦 **Color Boxes**: 4色（青、緑、黄、赤）の強調ボックス。
  - 🏷️ **Tags**: 分類や重要度を示すためのラベル。
  - ➡️ **Arrows**: 流れや推論を示すための矢印。
- 🖋️ **洗練されたタイポグラフィ**: Inter と BIZ UDPGothic を組み合わせた、読みやすくプロフェッショナルなフォント選定。
- 🔢 **自動ページネーション**: ヘッダーとフッターに洗練されたデザインのページ番号を表示。

## 🚀 インストール

Marp の設定（VS Code の `settings.json` など）で、カスタムテーマとして以下の URL を登録してください。

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

詳細な使い方は、[chiasm-usage-guide.md](./chiasm-usage-guide.md) または、それを PDF 出力した [chiasm-usage-guide.pdf](./chiasm-usage-guide.pdf) を参照してください。

## 🤖 AI によるスライド生成

付属の [chiasm-generation-prompt.md](./chiasm-generation-prompt.md) を LLM（ChatGPT, Claude 等）のプロンプトとして使用することで、Chiasm テーマに最適なスライド構成を自動生成できます。

1.  `chiasm-generation-prompt.md` の内容をコピーして AI に貼り付けます。
2.  スライドにしたい内容や構成案を AI に伝えます。
3.  AI が Chiasm の 2 段組みレイアウトやコンポーネントを駆使した Markdown コードを出力します。

## 🛠️ Canyon との主な違い

- 📐 **レイアウトの最適化**: 2段組み時の余白や境界線の調整。
- ➕ **コンポーネントの追加**: 矢印（uparrow, downarrow）や、より詳細なボックススタイルの追加。
- 💎 **デザインの微調整**: 文字サイズ、行間、色のコントラストなど、プレゼンテーションの可読性をさらに向上させました。

## 🧑‍💻 作者

- **mfujita47 (Mitsugu Fujita)** - [https://github.com/mfujita47](https://github.com/mfujita47)

## 📄 ライセンス

[MIT License](LICENSE)

## 📜 変更履歴

詳細は [CHANGELOG.md](CHANGELOG.md) を参照してください。
