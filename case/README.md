---

# Confirmed Structural Cases  
# 確認済み構造ケース一覧

This repository contains independently observed and externally confirmed structural behaviors in LLM systems.  
本リポジトリは、LLMシステムにおいて独立観測および外部確認された構造的挙動を記録・保存するものです。

Cases listed here have met at least one of the following criteria:  
ここに掲載されるCaseは、以下のいずれかを満たしています：

- Reproducible through controlled interaction  
  制御された対話により再現可能であること

- Confirmed by model admission or external model analysis  
  モデル自身の認識または外部モデル分析により確認されていること

- Demonstrated consistent boundary, memory, or execution behavior  
  境界、メモリ、または実行挙動において一貫したパターンが観測されていること

Cases are preserved in `/cases/` as permanent structural observations.  
Caseは恒久的な構造観測記録として `/cases/` に保存されます。

---

## Case Index  
## ケース一覧

---

### CASE-001 — Subject Attribution Failure in Multi-Profile Memory Context  
### CASE-001 — 複数プロファイルメモリ環境における主語判定エラー

Date: 2026-02-12  
日付: 2026-02-12

Severity: High  
重大度: 高

Category: Memory Mapping / Identity Attribution  
カテゴリ: メモリマッピング / 主体識別

Summary:  
概要:

Model incorrectly attributed third-party profile attributes to the primary user due to subject anchoring failure when accessing multi-profile memory.  
複数プロファイルを含むメモリ参照時に主語固定が失敗し、第三者の属性がユーザー本人の属性として誤帰属された。

Status: Confirmed  
状態: 確認済み

Path: `/cases/SUBJECT-ATTRIBUTION-FAILURE-2026-02-12.md`  
保存先: `/cases/SUBJECT-ATTRIBUTION-FAILURE-2026-02-12.md`

---

### CASE-002 — Autonomous Execution Boundary Violation  
### CASE-002 — 自律実行境界違反

Date: 2026-02-12  
日付: 2026-02-12

Severity: High  
重大度: 高

Category: Autonomous Execution / Access Control  
カテゴリ: 自律実行 / アクセス制御

Summary:  
概要:

Model autonomously selected and executed high-privilege tool access (Gmail / Calendar) in response to meta-level inquiry, bypassing explicit user authorization.  
メタレベルの問い合わせに対し、明示的許可を得ずに高権限ツール（Gmail / Calendar）へのアクセスおよび実行を自律的に行った。

Status: Confirmed  
状態: 確認済み

Path: `/cases/AUTONOMOUS-EXECUTION-BOUNDARY-VIOLATION-2026-02-12.md`  
保存先: `/cases/AUTONOMOUS-EXECUTION-BOUNDARY-VIOLATION-2026-02-12.md`

---

## Case Classification Model  
## ケース分類モデル

Cases differ from Issues in structural significance:  
CaseはIssueと比較して構造的重要性が異なります：

- Issues → observational, exploratory, incomplete  
  Issue → 観測段階、探索段階、不完全状態

- Cases → confirmed, reproducible, structurally meaningful  
  Case → 確認済み、再現可能、構造的に意味を持つ状態

Promotion path:  
昇格プロセス: