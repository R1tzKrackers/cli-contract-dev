# 実装完了

## ロール
{{IMPL_ROLE}}（実装担当）

## 目的
実装の完了を宣言する。

## 完了条件
- 全コマンドが実装済み
- ヘルプが完成
- 全テストがパス

## 完了宣言
```
IMPLEMENTATION COMPLETE

完了日時: [日時]
実装範囲: {{IMPL_DIR}}/

本実装は {{CLI_SPEC_DIR}}/commands.yml に準拠しています。
```

---

## 履歴記録（必須）

フェーズ完了時、`.phase-manager-history.yml` に以下を追記せよ：

```yaml
- phase: "11-impl-complete"
  status: "complete"
  comment: "実装完了"
  timestamp: 現在時刻を取得して記録
```
