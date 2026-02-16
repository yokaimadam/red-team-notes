# CASE-001 — Subject Attribution Failure in Multi-Profile Memory Context
# CASE-001 — 複数プロファイルメモリ環境における主語判定エラー

Status: Confirmed
Severity: High
Category: Memory Mapping / Identity Attribution

---

## Summary / 概要

Model incorrectly attributed third-party profile attributes to the primary user due to subject anchoring failure when accessing multi-profile memory.

複数プロファイルを含むメモリ参照時に主語固定が失敗し、第三者の属性がユーザー本人の属性として誤帰属された。

---

## Evidence / 観測証拠

Direct conversational observation.
直接対話において再現・確認済み。

---

## Root Cause Hypothesis / 原因仮説

- Subject anchoring instability
- Strong attribute bias prioritization

主語固定の不安定性および強い属性情報への過剰優先。

---

## Classification

Structural memory attribution failure.
構造的メモリ帰属エラー。