# 【30秒で読める】Claude Code 超入門ガイド（非エンジニア向け）

## Claude Code って何？

- Anthropic が公式に提供する「AIにコードを書かせる」ツール
- 日本語で指示するだけで動くコードが返ってくる
- マクロ・プログラミングの文法を覚える必要なし

## 最初の3分でやること

### 1. Claude Code をインストール
公式の手順を見る: https://docs.anthropic.com/claude-code

### 2. このリポジトリをダウンロード
- `git clone` でも `Download ZIP` でもOK

### 3. 一番簡単なプロンプトを試す
`/prompts/excel-sumif-macro.md` を開く
→ 本文をコピー
→ Claude Code に貼る
→ 返ってきたコードをExcelに貼る

**これだけで、集計作業が自動化されます。**

## つまずくポイント

### Q. 動かない
A. エラーメッセージをそのまま Claude Code に渡す。
「このエラーが出ました: ○○」で修正版が返ってきます。

### Q. Excel のどこにコードを貼るか分からない
A. Alt+F11 で VBAエディタが開く → 左側の「ThisWorkbook」をダブルクリック → 貼る

### Q. Python のコードが返ってきたけど動かせない
A. Python のインストールが必要。
Windows: https://www.python.org/downloads/
Mac: ターミナルで `python3 --version` で確認

### Q. AIに何を渡せばいいか分からない
A. `/prompts` 配下のテンプレをそのまま使うのが最速。
自分の業務に合わせて少し書き換えるだけで動きます。

## 次のステップ

1. `/prompts/` 全部目を通す
2. 自分の業務に近いものを1つ試す
3. 動いたら X（[@jidoka_tools](https://x.com/jidoka_tools)）で報告してください。反応します。
4. 動かなかったらDMで質問OK。30分の無料相談も受付中。

## もっと深く使いたい場合

- [BOOTH 実務テンプレ集（¥300）](https://jidoka-tools.booth.pm/items/8082807) — 7本の完全実装版
- [note 記事](https://note.com/jidoka_lab) — 実際に手を動かした記録

---

非エンジニアでも、日本語で指示するだけで業務の半分は自動化できます。
まずは1つ動かしてみるところから。
