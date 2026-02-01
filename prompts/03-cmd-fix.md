# コマンド修正

## ロール
{{DESIGN_ROLE}}（設計担当）

## 目的
検証で発見された問題を修正する。

## 入力
- `{{CLI_SPEC_DIR}}/verify-report.md`
- レビューフィードバック

## 成果物
- `{{CLI_SPEC_DIR}}/commands.yml` の修正
- `{{CLI_SPEC_DIR}}/options.yml` の修正

---

## 履歴記録（必須）

フェーズ完了時、`.phase-manager-history.yml` に以下を追記せよ：

```yaml
- phase: "03-cmd-fix"
  status: "complete"
  comment: "修正内容を1行で"
  timestamp: 現在時刻を取得して記録
```
