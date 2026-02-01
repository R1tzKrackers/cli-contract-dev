# プロジェクト設定

## 目的
project-config.yml をプロジェクトに合わせてカスタマイズする。

## 成果物
- `project-config.yml` の更新

## 指示
1. プロジェクト名を設定
2. ディレクトリ構成を確認・調整
3. ロール名を必要に応じて変更

## 設定項目
```yaml
project:
  name: "{{PROJECT_NAME}}"

directories:
  cli_spec: docs/cli       # CLI仕様書
  impl: src                # 実装コード
  test: tests              # テストコード

roles:
  design: Designer         # コマンド設計担当
  impl: Developer          # 実装担当
```

---

## 履歴記録（必須）

フェーズ完了時、`.phase-manager-history.yml` に以下を追記せよ：

```yaml
- phase: "00c-project-config"
  status: "complete"
  comment: "設定内容を1行で"
  timestamp: 現在時刻を取得して記録
```
