# 詳細設計

## ロール
{{DESIGN_ROLE}}（設計担当）

## 目的
各コマンドの詳細仕様と入出力を設計する。

## 入力
- `{{CLI_SPEC_DIR}}/commands.yml`

## 成果物
- `{{CLI_SPEC_DIR}}/detail/` - コマンド詳細仕様
- `{{CLI_SPEC_DIR}}/detail/io-spec.yml` - 入出力仕様
- `{{CLI_SPEC_DIR}}/detail/errors.yml` - エラーコード定義

## 指示
1. 各コマンドの処理フローを定義
2. 入力バリデーションルールを定義
3. 出力フォーマット（JSON/Text/Table）を定義
4. 終了コードを定義
5. エラーメッセージを定義

---

## 履歴記録（必須）

フェーズ完了時、`.phase-manager-history.yml` に以下を追記せよ：

```yaml
- phase: "04-detail-design"
  status: "complete"
  comment: "設計内容を1行で"
  timestamp: 現在時刻を取得して記録
```
