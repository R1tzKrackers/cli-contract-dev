# 実装検証

## ロール
{{IMPL_ROLE}}（実装担当）

## 目的
実装がコマンド仕様に準拠しているか検証する。

## 入力
- `{{CLI_SPEC_DIR}}/commands.yml`
- `{{IMPL_DIR}}/`

## 検証項目
1. 全コマンドが実装されているか
2. オプションが仕様通りか
3. 出力フォーマットが正しいか
4. 終了コードが正しいか
5. ヘルプが表示されるか

## 成果物
- 検証レポート

---

## 履歴記録（必須）

フェーズ完了時、`.phase-manager-history.yml` に以下を追記せよ：

```yaml
- phase: "10-impl-verify"
  status: "complete"
  comment: "検証結果を1行で"
  timestamp: 現在時刻を取得して記録
```
