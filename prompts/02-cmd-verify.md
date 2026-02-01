# コマンド検証

## ロール
{{DESIGN_ROLE}}（設計担当）

## 目的
コマンド設計の整合性と完全性を検証する。

## 入力
- `{{CLI_SPEC_DIR}}/commands.yml`
- `{{CLI_SPEC_DIR}}/options.yml`

## 検証項目
1. コマンド名の重複がないか
2. オプション名の重複がないか
3. 必須引数が明確か
4. サブコマンド階層が適切か

## 成果物
- `{{CLI_SPEC_DIR}}/verify-report.md` - 検証レポート

---

## 履歴記録（必須）

フェーズ完了時、`.phase-manager-history.yml` に以下を追記せよ：

```yaml
- phase: "02-cmd-verify"
  status: "complete"
  comment: "検証結果を1行で"
  timestamp: 現在時刻を取得して記録
```
