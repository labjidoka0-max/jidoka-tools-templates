# jidoka-tools-templates

> 非エンジニアの営業職が、Claude Code で業務を自動化したときの実物テンプレ・プロンプト・スキル集。

[![BOOTH](https://img.shields.io/badge/BOOTH-無料スターターキット-orange)](https://jidoka-tools.booth.pm/items/8104584)
[![X](https://img.shields.io/badge/X-@jidoka__tools-black)](https://x.com/jidoka_tools)
[![note](https://img.shields.io/badge/note-jidoka__lab-green)](https://note.com/jidoka_lab)

## 🎯 このリポジトリの目的

Claude Code を「日本語で指示するだけで動かす」運用を、非エンジニア営業職が1ヶ月回した実録です。

**コードが書けない人** に向けて、**コピペで動くテンプレ** をオープンソース化しています。

## 📦 収録内容

### `/prompts` — 日本語プロンプトサンプル
- `excel-sumif-macro.md` — 店舗別×月別でSUMIFしてピボット風に
- `meeting-notes-structure.md` — 会議メモ → 決定/宿題/期限 の3列表化
- `email-reply-3patterns.md` — 受信メール → 返信下書き3パターン生成
- `expense-csv-classify.md` — 経費CSV → 科目別自動仕分け
- `weekly-report-generator.md` — Excel数値 → 文章化された週次レポート
- `excel-aggregate-ja.md` — 得意先別 合計＋並び替え（入門サンプル）
- `excel-transcribe-ja.md` — テンプレへの定型転記（入門サンプル）
- `excel-format-ja.md` — 電話番号・日付の整形（入門サンプル）

### `/skills` — Claude Code SKILL.md サンプル
- `excel-automation.md` — Excel系業務自動化の標準フロー
- `document-structuring.md` — 議事録・メモの構造化
- `sales-toolkit.md` — 営業職向けツール集

### `/examples` — 実際に動かした成果物
- `sumif-macro.vba` — 実行5秒の売上集計マクロ
- `expense-classifier.py` — 経費仕分けPythonスクリプト
- `weekly-report-template.xlsx` — 週次レポート雛形（※別途BOOTH配布）

### `/docs` — ハウツー記事
- `beginner-guide.md` — 非エンジニアが最初に読むべき1ページ
- `troubleshooting.md` — エラー発生時の対処集
- `faq.md` — よくある質問

## 🚀 使い方（30秒）

1. このリポジトリを `git clone` または ZIP ダウンロード
2. `/prompts` の中から自分の業務に近いものを選ぶ
3. そのテキストをコピーして Claude Code に渡す
4. 返ってきたコードをExcelやPythonに貼るだけ

詳細: [docs/beginner-guide.md](docs/beginner-guide.md)

## 📊 削減実績（自己計測）

| 業務 | 手作業 | Claude Code化後 |
|------|-------|--------------|
| 月次売上集計（SUMIF版） | 40分 | 5秒 |
| 議事録 構造化 | 25分 | 30秒 |
| 経費CSV 仕分け | 30分 | 10秒 |
| 週次レポート 文章化 | 60分 | 2分 |

**合計 約月12時間の手作業削減。**

## 🔗 関連リンク

- 🆓 [無料スターターキット（BOOTH）](https://jidoka-tools.booth.pm/items/8104584)
- 📘 [実務テンプレ7本セット ¥300（BOOTH）](https://jidoka-tools.booth.pm/items/8082807)
- 📝 [公開記事（note）](https://note.com/jidoka_lab)
- 💬 [DM相談（X）](https://x.com/jidoka_tools) — 30分無料相談受付中

## 📝 ライセンス

MIT License. 業務利用・改変・再配布すべて自由です。

## 🤝 コントリビューション歓迎

- 動かなかった → Issue
- 別パターン試した → Pull Request
- こんなプロンプト欲しい → Discussions

**非エンジニアでも貢献OK。** 「このプロンプトで動きました」報告も歓迎です。

---

## 運営者について

非エンジニアの営業職が、2026年春からClaude Codeで業務自動化を実践しています。
プログラミングは全くわからない、マクロも書けない、そんな立場でどこまで自動化できるかの実験ログを公開しています。

- X: [@jidoka_tools](https://x.com/jidoka_tools)
- note: [note.com/jidoka_lab](https://note.com/jidoka_lab)
- BOOTH: [jidoka-tools.booth.pm](https://jidoka-tools.booth.pm/)
