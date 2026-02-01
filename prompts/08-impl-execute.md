# 実装

## ロール
{{IMPL_ROLE}}（実装担当）

## 目的
コマンド仕様に基づいてCLIを実装する。

## 入力
- `{{CLI_SPEC_DIR}}/commands.yml`
- `{{CLI_SPEC_DIR}}/detail/`

## 成果物
- `{{IMPL_DIR}}/` - CLIコマンド実装

## 指示
1. コマンドパーサーを実装
2. 各コマンドのハンドラを実装
3. オプション処理を実装
4. 入力バリデーションを実装
5. 出力フォーマッターを実装
6. エラーハンドリングを実装

## 注意事項
- 仕様書に記載のないコマンドを追加しない
- 終了コードを仕様通りに設定する

---

## 履歴記録（必須）

フェーズ完了時、`.phase-manager-history.yml` に以下を追記せよ：

```yaml
- phase: "08-impl-execute"
  status: "complete"
  comment: "実装内容を1行で"
  timestamp: 現在時刻を取得して記録
```
