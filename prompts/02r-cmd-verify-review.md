# コマンド検証レビュー

## 目的
コマンド検証結果の人間レビューを実施する。

## レビュー対象
- `{{CLI_SPEC_DIR}}/verify-report.md`

## 判定
- **承認**: 次フェーズ（詳細設計）へ進む
- **差し戻し**: コマンド修正フェーズに戻る
- **再設計**: コマンド設計フェーズに戻る

---

## 履歴記録（必須）

フェーズ完了時、`.phase-manager-history.yml` に以下を追記せよ：

```yaml
- phase: "02r-cmd-verify-review"
  status: "complete"  # または "reject"（差し戻しの場合）
  comment: "レビュー結果を1行で"
  target: "03-cmd-fix"  # 差し戻し先（rejectの場合のみ）
  timestamp: 現在時刻を取得して記録
```
