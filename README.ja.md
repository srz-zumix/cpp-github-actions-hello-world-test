# cpp-github-actions-hello-world

C++ GitHub Actions の Hello World テンプレート

## 使い方

### Repository の作成

[Start](https://github.com/new?template_owner=srz-zumix&template_name=cpp-github-actions-hello-world&owner=%40me&name=cpp-github-actions-hello-world&description=My+clone+repository&visibility=public)

1. **Start** 右クリックし新規タブで開きます
1. 開いたタブに移動します。おおよその入力項目は自動でセットされています
   - Owner を選択してください
   - Public リポジトリを作成してください（Private の場合は Actions の実行に[制限](https://docs.github.com/ja/billing/managing-billing-for-github-actions/about-billing-for-github-actions)がかかります）
   - 最後に最下部にある `Create repository` ボタンをクリックします

### ワークフローの作成

1. リポジトリの「Actions」タブを開きます
1. `New workflow` ボタンをクリックします
1. `Suggested for this repository` に `C/C++ with Make` があると思いますのでそちらの `Configure` をクリックします
1. ワークフローの雛形ができるのでそれを元に編集します
   - `configure` と `make distcheck` の step は使わないので削除します
   - `make check` の step の name と run を `make run` に変更します
1. Commit してプルリクエストを作成します.
   - `Commit Changes..` をクリックしてください。コミット作成のポップアップが表示されます
   - `Create a new branch for this commit and start a pull request` を選択します
   - ブランチ名を入力します。そのままでも問題ありません
   - ポップアップ下部の `Commit Changes` をクリックします
   - `Open a pull request` ページが開くので、詳細を記入したのちに `Create pull request` ボタンをクリックします
1. Checks が完了するのを待ちます
1. `All checks have passed` になれば成功です
   - `Show all checks` をクリックすると Checks 一覧が表示されます
   - C/C++ CI / build (pull_request) の `Details` をクリックし開きます
   - ログに「Hello GitHub Actions!」と出力されているのを確認してください

## オススメチュートリアル

- [skills/hello-github-actions](https://github.com/skills/hello-github-actions)
