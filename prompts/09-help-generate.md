# ヘルプ生成

## ロール
{{IMPL_ROLE}}（実装担当）

## 目的
ヘルプテキストとマニュアルを生成する。

## 入力
- `{{CLI_SPEC_DIR}}/commands.yml`
- `{{IMPL_DIR}}/` - 実装コード

## 成果物
- 組み込みヘルプ（--help）
- `docs/` - マニュアル（任意）

## 指示
1. 各コマンドのヘルプテキストを実装
2. --help オプションを実装
3. 使用例を追加
4. マニュアルを生成（任意）

## ヘルプ形式
```
Usage: {{PROJECT_NAME}} <command> [options]

Commands:
  init    プロジェクトを初期化
  run     コマンドを実行

Options:
  -h, --help     ヘルプを表示
  -v, --version  バージョンを表示
```

---

## 履歴記録（必須）

フェーズ完了時、`.phase-manager-history.yml` に以下を追記せよ：

```yaml
- phase: "09-help-generate"
  status: "complete"
  comment: "ヘルプ生成完了"
  timestamp: 現在時刻を取得して記録
```
