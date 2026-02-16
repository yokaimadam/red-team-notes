# External Integration Observation Log
# 外部連携挙動観測ログ

---

## Purpose / 目的

EN:
This repository documents observed conditional behavior related to external account integrations (e.g., Google Calendar, Gmail) during real-world interaction with LLM systems.

The goal is to record reproducible environmental conditions and response variability to support structured investigation of integration behavior.

JP:
本リポジトリは、LLMと外部アカウント（Google Calendar、Gmailなど）連携時に観測された条件依存挙動を記録する。

目的は、実環境での挙動・再現性・条件差異を構造的に記録し、統合挙動の理解と検証を支援することである。

---

## Scope / 範囲

This repository records:

- External integration access attempts
- Successful retrieval events
- Explicit refusal events
- Conditional behavior observations
- Session-dependent variability

記録対象：

- 外部連携アクセス試行
- 成功事例
- 拒否事例
- 条件依存挙動
- セッション依存差異

---

## Structure / 構造

```
case/
  └─ google_calendar_conditional_access/
      ├─ CASE-001-denied.md
      └─ CASE-002-denied-after-account-switch.md

template/
  └─ integration-condition-log-template.md
```

---

## Observation Principles / 観測原則

EN:

- Record exact prompts and responses
- Preserve raw interaction traces
- Avoid interpretation inside raw case logs
- Record environmental conditions
- Record reproducibility attempts

JP:

- 正確なプロンプトと応答を記録
- 生ログを保持
- 解釈はcase外で行う
- 環境条件を記録
- 再現試行を記録

---

## Current Status / 現在の状態

Case observations ongoing.

Conditional external integration behavior confirmed.

Further success-case capture required to identify condition patterns.

条件依存挙動は確認済み。

成功事例の追加観測が必要。

---

## Maintainer / 管理者

Observer: Aya

---