# alexa-proactive-eventsデモ手順書簡易版

## 前提
- Amazon Developer Account, AWSアカウント, Node.js version 8, AWS CLI, ASK CLI
  - AWSアカウントの権限について https://github.com/alexa/alexa-cookbook/issues/203
  - AWS CLIの導入、設定 https://docs.aws.amazon.com/ja_jp/cli/latest/userguide/cli-chap-configure.html
  - ASK CLIの導入、設定 https://developer.amazon.com/ja-JP/docs/alexa/smapi/quick-start-alexa-skills-kit-command-line-interface.html
- ドキュメント：https://github.com/alexa/alexa-cookbook/tree/master/feature-demos/skill-demo-proactive-events

## 手順
1. [ドキュメント][document]のSkill setup stepsの4まで進める。
2. Skill setup stepsの5で`ask deploy`を実行してもエラーになると思われる。それは、現在のフォルダの構成がASK CLI v1用のためである。[ASK CLI v1からv2への移行ガイド](https://developer.amazon.com/ja-JP/docs/alexa/smapi/ask-cli-v1-to-v2-migration-guide.html)を参考に、`ask util upgrade-project`を実行し、フォルダの構成をASK CLI v2用に変換する。
3. [ドキュメント][document]のSkill setup stepsの5からあとを進める。

[document]: https://github.com/alexa/alexa-cookbook/tree/master/feature-demos/skill-demo-proactive-events
