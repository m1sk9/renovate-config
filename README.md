# lis2a/renovate-config

my renovate config

## Usage

```json
{
    "extends": ["github>lis2a/renovate-config"]
}
```

## Settings

リポジトリの `renovate.json` に設定を上書きすることが出来ます。

設定方法の詳細は Renovate Docs を確認してください。

[Configuration Options - Renovate Docs](https://docs.renovatebot.com/configuration-options/)

----

#### Note

- [Faker.js](https://snyk.io/blog/npm-faker-package-open-source-libraries/) や [core.js](https://www.itmedia.co.jp/news/articles/2201/11/news160.html) , [peacenotwar](https://snyk.io/blog/peacenotwar-malicious-npm-node-ipc-package-vulnerability/) の件以降、基本的に私は npm コミュニティを信頼していないため、最低でもリリースから3日経過するまで Renovate が作成しないようにしています。(全てのライブラリがそうとは思ってないが...)
- メジャーアップデート、ロールバック が行われたライブラリは自動Merge、 自動Approveされません。
- ロールバック が行われたライブラリは `fix(deps)` が prefix としてプルリクエストが作成されます。
- 毎週月曜日のAM 5:00にアップデートが行われます。
  - セキュリティパッチは随時行われます。
