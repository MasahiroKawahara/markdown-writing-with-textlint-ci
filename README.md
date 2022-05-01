# markdown-writing-with-textlint-ci
- ブログ:
- サンプルプルリクエスト: https://github.com/MasahiroKawahara/markdown-writing-with-textlint-ci/pull/5

## ファイル構成

| Path                                 | Description                                   |
| --                                   | --                                            |
| `README.md`                          | このファイル                                  |
| `contents/`                          | Markdown文書格納先ディレクトリ                |
| `.textlintrc`                        | テキスト校正ルール                            |
| `.github/workflows/run-textlint.yml` | テキスト校正自動化のワークフロー              |
| `package-lock.json`                  | (上記ワークフロー内の nodeセットアップで利用) |
| `package.json`                       | (上記ワークフロー内の nodeセットアップで利用) |

## 執筆者向けマニュアル
### 最初にやること

このリポジトリをローカル環境に複製 ( `git clone` ) してください。

### 執筆活動の流れ

1. ローカルを最新にする ( `git switch main; git pull` )
2. 執筆作業ブランチを作成 ( 例: `git branch --create write-xxx-section` )
3. 執筆作業ブランチに移動 ( 例: `git switch write-xxx-section` )
4. **執筆活動！**
5. 変更をコミット (例: `git add contents/xxx.md; git commit -m "xxx章記載"` )
6. リモートリポジトリへプッシュ (例: `git push origin write-xxx-section` )
7. プルリクエストを作成 (GitHubリポジトリの `Pull request > New pull request` )
8. レビューが「OK」になるまで `修正 → コミット →　プッシュ → 再レビュー` を繰り返す
9. 【完了】 main ブランチにマージされます ( `1.` に戻る )
