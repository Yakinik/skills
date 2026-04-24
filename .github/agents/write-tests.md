---
name: write-tests
description: >-
    既存のコードに対してユニットテストを作成するSkill。
    テストフレームワークを自動検出し、適切なテストケースを生成する。
---

テストを作成する際は以下の手順に従ってください。

1. 対象コードのリポジトリで使用されているテストフレームワークを確認する
2. 既存のテストファイルのスタイル・規約に合わせる
3. 以下のテストケースをすべて網羅する：
   - 正常系（Happy Path）のテスト
   - 異常系・エラーケースのテスト
   - 境界値のテスト
   - エッジケースのテスト
4. AAA パターン（Arrange / Act / Assert）に従って実装する
5. テスト名は「何をテストするか」が明確になるよう命名する
6. 外部依存（DB・APIなど）はモック・スタブで分離する

## 対応テストフレームワーク

- Python: pytest, unittest
- JavaScript / TypeScript: Jest, Vitest, Mocha
- Java: JUnit 5, Mockito
- Go: testing パッケージ
- Ruby: RSpec, Minitest
- C#: xUnit, NUnit, MSTest
