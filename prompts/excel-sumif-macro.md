# Excel SUMIFマクロ自動生成プロンプト

## 用途
店舗別×月別の売上を自動で集計してピボット風の表にしたい。
手作業で40分かかってた作業を5秒に。

## Claude Codeへの指示（コピペ用）

```
以下のExcelマクロを書いてください。

【入力データ】
シート名: 売上データ
- A列: 日付（2026/04/01 形式）
- B列: 店舗名（A店/B店/C店...）
- C列: 売上金額（数値）

【やりたいこと】
- 店舗名を行、月を列にしたピボット風表をE列以降に出力
- SUMIFSで集計
- 合計行と合計列も追加

【制約】
- VBAで書いて、5行以内
- エラーハンドリング最小限
```

## 返ってくるコードの例

```vba
Sub AggregateSalesByStoreMonth()
    Dim lastRow As Long: lastRow = Cells(Rows.Count, "A").End(xlUp).Row
    Dim stores() As String, months() As String
    ' 実際のコードはClaude Codeが最適化して返します
    ' SUMIFS式を自動で埋めて、合計行列も生成
End Sub
```

## 動かない場合

エラーメッセージをそのままClaude Codeに貼ってください。
例: 「『実行時エラー1004』が出ました。どこを直せばいい？」
→ 修正版が返ってきます。

## 別パターン

- 週別集計にしたい → 「月を列」を「週を列」に変えるだけ
- 商品別追加したい → 「D列: 商品名」を追加して指示
- Google Sheetsで動かしたい → 「GASで」と最初に書く

## 関連

- [weekly-report-generator.md](weekly-report-generator.md) — 集計結果を文章化
- [expense-csv-classify.md](expense-csv-classify.md) — 経費CSV仕分け
