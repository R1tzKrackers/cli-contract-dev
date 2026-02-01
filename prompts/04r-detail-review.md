# 詳細設計レビュー

## 目的
詳細設計成果物の人間レビューを実施する。

## レビュー対象
- `{{CLI_SPEC_DIR}}/detail/`

## レビュー観点
1. 実装に必要な情報が揃っているか
2. エラーハンドリングが網羅されているか
3. 出力フォーマットが適切か

## 判定
- **承認**: 次フェーズ（引継ぎ判定）へ進む
- **差し戻し**: 詳細設計フェーズに戻る

---

## 履歴記録（必須）

フェーズ完了時、`.phase-manager-history.yml` に以下を追記せよ：

```yaml
- phase: "04r-detail-review"
  status: "complete"  # または "reject"（差し戻しの場合）
  comment: "レビュー結果を1行で"
  target: "04-detail-design"  # 差し戻し先（rejectの場合のみ）
  timestamp: 現在時刻を取得して記録
```
