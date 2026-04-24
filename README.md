# skills

コーディングエージェント（主にClaude Code / GitHub Copilot コーディングエージェント）のSkillsを置くリポジトリです。

## 概要

このリポジトリには、コーディングエージェントが特定のタスクをより効果的に実行するための **Skills（スキル）** を管理しています。

Skillsは `.github/agents/` ディレクトリ内のMarkdownファイルとして定義されており、エージェントが呼び出せるカスタム能力・ドメイン知識を提供します。

## Skillsの一覧

| Skill名 | 説明 |
|--------|------|
| [code-review](skills/code-review.md) | コードレビューを実施し、品質・セキュリティ・可読性を評価する |
| [write-tests](skills/write-tests.md) | 既存コードに対してユニットテストを作成する |
| [refactor](skills/refactor.md) | コードのリファクタリングを行い、品質を改善する |

## Skillsの追加方法

1. `skills/` ディレクトリに新しい `<skill-name>.md` ファイルを作成する
2. YAMLフロントマターでスキルのメタデータを記述する
3. スキルの説明・手順・注意事項をMarkdownで記述する

### Skillファイルの形式

```markdown
---
name: skill-name
description: >-
    スキルの短い説明
---

# スキルのタイトル

スキルの詳細な説明と手順...
```

## 参考

- [GitHub Copilot コーディングエージェントのドキュメント](https://docs.github.com/en/copilot/concepts/agents/copilot-coding-agent)
- [開発環境のカスタマイズ](https://docs.github.com/en/copilot/customizing-copilot/customizing-the-development-environment-for-copilot-coding-agent)
