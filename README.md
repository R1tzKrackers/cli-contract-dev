# CLI Contract Framework

**CLI開発フレームワーク / CLI Development Framework**

[![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)]()
[![Phase Manager](https://img.shields.io/badge/requires-Phase%20Manager-green.svg)]()

---

## 概要 / Overview

CLI Contract Frameworkは、コマンドライン設計を起点とした開発ワークフローを提供するフレームワークです。
コマンド設計から実装、ヘルプ生成までの一貫したフローを定義します。

*CLI Contract Framework provides a command-line-first development workflow.
It defines a consistent flow from command design to implementation and help generation.*

---

## 特徴 / Features

- **コマンド駆動設計** - コマンド体系設計を起点とした開発フロー
  *Command-Driven Design - Development flow starting from command structure design*

- **契約凍結** - コマンド仕様凍結後の変更を防止
  *Contract Freeze - Prevents specification changes after command design completion*

- **ヘルプ生成** - コマンド仕様に基づくヘルプ自動生成支援
  *Help Generation - Supports help generation based on command specification*

---

## ワークフロー / Workflow

```
[Setup]
  00c-project-config    プロジェクト設定 / Project Configuration
       |
[Design - Command]
  01-cmd-design         コマンド設計 / Command Design
  01r-cmd-review        コマンド設計レビュー / Command Design Review
  02-cmd-verify         コマンド検証 / Command Verification
  02r-cmd-verify-review コマンド検証レビュー / Command Verification Review
  03-cmd-fix            コマンド修正（任意）/ Command Fix (optional)
       |
[Design - Detail]
  04-detail-design      詳細設計 / Detail Design
  04r-detail-review     詳細設計レビュー / Detail Review
       |
[Handoff]
  05-handoff-check      引継ぎ判定 / Handoff Check
  06-design-freeze      契約凍結 / Contract Freeze
       |
[Implementation]
  07-impl-start         実装開始 / Implementation Start
  08-impl-execute       実装 / Implementation Execute
  09-help-generate      ヘルプ生成 / Help Generation
  10-impl-verify        実装検証 / Implementation Verification
  10r-impl-verify-review 実装検証レビュー / Implementation Review
  11-impl-complete      実装完了 / Implementation Complete
```

---

## ディレクトリ構成 / Directory Structure

```
cli-contract-dev/
├── framework.yml      # フレームワークマニフェスト / Framework manifest
├── prompts/           # フェーズ別プロンプト / Phase-specific prompts
└── templates/         # テンプレート / Templates
    └── AGENTS.md.template
```

---

## 使用方法 / Usage

### 前提条件 / Prerequisites

- [Phase Manager](https://github.com/R1tzKrackers/phase-manager) がインストール済みであること

### セットアップ / Setup

1. Phase Managerの初期化フェーズで本フレームワークを選択
2. `project-config.yml` でプロジェクト固有の設定を行う

---

## 変数 / Variables

| 変数 / Variable | 説明 / Description |
|-----------------|---------------------|
| `{{PROJECT_NAME}}` | プロジェクト名 / Project name |
| `{{DESIGN_ROLE}}` | 設計担当ロール名 / Design role name |
| `{{IMPL_ROLE}}` | 実装担当ロール名 / Implementation role name |
| `{{CLI_SPEC_DIR}}` | CLI仕様書ディレクトリ / CLI spec directory |
| `{{IMPL_DIR}}` | 実装ディレクトリ / Implementation directory |
| `{{TEST_DIR}}` | テストディレクトリ / Test directory |

---

## ライセンス / License

MIT License

---

## 関連 / Related

- [Phase Manager](https://github.com/R1tzKrackers/phase-manager) - ワークフロー管理ツール
