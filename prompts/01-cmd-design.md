# コマンド設計

## ロール
{{DESIGN_ROLE}}（設計担当）

## 目的
CLIのコマンド体系とオプションを設計する。

## 入力
- プロジェクト要件
- ユーザーストーリー

## 成果物
- `{{CLI_SPEC_DIR}}/commands.yml` - コマンド一覧
- `{{CLI_SPEC_DIR}}/options.yml` - グローバルオプション

## 指示
1. メインコマンドを定義
2. サブコマンド階層を設計
3. 各コマンドのオプションを定義
4. 入出力形式を定義

## 出力形式
```yaml
# {{CLI_SPEC_DIR}}/commands.yml
commands:
  - name: init
    description: プロジェクトを初期化
    options:
      - name: --force
        short: -f
        description: 強制的に初期化
    subcommands: []

  - name: run
    description: コマンドを実行
    arguments:
      - name: target
        required: true
        description: 実行対象
```

## 注意事項
- POSIXスタイルのオプション命名
- ヘルプテキストの一貫性
- エラーメッセージの標準化

---

## 履歴記録（必須）

フェーズ完了時、`.phase-manager-history.yml` に以下を追記せよ：

```yaml
- phase: "01-cmd-design"
  status: "complete"
  comment: "設計内容を1行で"
  timestamp: 現在時刻を取得して記録
```
