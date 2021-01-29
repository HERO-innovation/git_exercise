# git_exercise
Gitの練習用


## GitHub 運用
### ブランチ
| ブランチ名 | 説明 | |
| --- | --- |--- |
| `master` | 常に本番環境にデプロイ可能。 | |
| `develop` | Default ブランチ。常にステージング環境にデプロイ可能。 | |
| `feature/${yearmonth}/${username}/content_description` | 通常の作業を目的とし `develop` より派生するブランチ。 | |
| `staging` | ステージング用のブランチ。本番と同じ環境。develop確認OKの場合にマージする | 練習なので作ってない |
| `hotfix/${yearmonth}/${username}/content_description` | 障害対応は急な作業を目的とし `master` より派生するブランチ。 | 練習なのでやらない |

### 作業〜マージする場合
* developブランチの最新から(pullする)、自分の作業用にfeatureブランチを作りましょう
* featureブランチで作業後、commit、 featureブランチをpushしてください。
  * (名前の例) feature/20210129/username/update_index
* featureブランチはdevelopブランチにマージします
* featureブランチをdevelopブランチにマージする場合は、プルリクエストを作成します。
  * プルリクエストはprotection ruleにより2名からapproveが必要です。
* 2名からOKが出た場合は本人がdevelopにマージします。

### コミットルール
- コミットコメントは日本語で端的に書く
- 出来るだけ単一コミットに複数の更新を入れない
