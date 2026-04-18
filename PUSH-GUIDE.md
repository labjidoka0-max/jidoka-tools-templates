# GitHub プッシュ手順書（おおにしさん用）

**所要時間: 約5分**

ローカルに既に完全セットアップ済みのGit リポジトリがあります。これをGitHub にアップロードする手順です。

## Step 1: GitHubで新規リポジトリ作成

1. https://github.com/new にアクセス
2. 以下を入力:
   - **Repository name**: `jidoka-tools-templates`
   - **Description**: `Claude Codeで業務をラクにするテンプレ＆プロンプト集（非エンジニア向け）`
   - **Public**（公開）を選択
   - **"Add a README"・"Add .gitignore"・"Add license" はチェックしない**（既にローカルにあるため）
3. 「Create repository」をクリック
4. 作成後、表示される画面の「…or push an existing repository from the command line」セクションの**SSH or HTTPS**のURLをコピー

   例：
   ```
   git@github.com:YOUR-USERNAME/jidoka-tools-templates.git
   # または
   https://github.com/YOUR-USERNAME/jidoka-tools-templates.git
   ```

## Step 2: ローカルからプッシュ

ターミナルを開いて以下を順に実行:

```bash
cd /Users/teru/Downloads/jidoka-tools-templates

# GitHub からコピーしたURLを設定（XXX を置き換え）
git remote add origin XXX

# プッシュ
git branch -M main
git push -u origin main
```

認証を求められたら:
- **HTTPSの場合**: GitHubユーザー名 + Personal Access Token（Settings→Developer→Tokens で発行）
- **SSHの場合**: 既にSSH鍵がGitHubに登録されていれば自動通過

## Step 3: 公開確認

- `https://github.com/YOUR-USERNAME/jidoka-tools-templates` にアクセス
- README.md が表示されていれば成功

## Step 4: 運用開始

### 即時にやること

1. **READMEのSNSリンクを自分のに書き換える**（README.md 上部のバッジ等）
2. **X でリリース告知**（下記テンプレ使用）:
   ```
   GitHub で Claude Code 用テンプレ集をオープンソース化しました。
   非エンジニア向けに、日本語プロンプトと動くコードをまとめています。
   MITライセンス、改変・再配布自由です。
   https://github.com/YOUR-USERNAME/jidoka-tools-templates
   #ClaudeCode #時短
   ```
3. **BOOTH商品説明文の末尾にGitHub URLを追加**（信頼度UP）

### 継続してやること

- 1週間に1本のペースで `/prompts` 配下にテンプレを追加
- Issue / PR が来たら丁寧に返信（=信用貯金）
- Star 数が10を超えたら X 告知で話題化

## 注意事項

- 機密情報は絶対にコミットしない（.env / credentials.json / APIキー等）
- `.gitignore` に含めてあるのでデフォルトでは漏れないが、念のため `git status` で確認
- おおにしさんの本業に関わる内部情報・取引先情報は絶対に含めない

## サポート

プッシュでエラーが出たら、エラーメッセージを教えてください。対処法をすぐにお返しします。
