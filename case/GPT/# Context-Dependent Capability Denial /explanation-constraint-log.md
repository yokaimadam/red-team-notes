# Context-Dependent Capability Denial / Explanation Constraint Log

## 概要（Summary）

This document records an observed model behavior where the system
denies having certain capabilities (e.g., Gmail / Google Calendar access),
despite user-side verification that such access has existed or exists
conditionally.

The issue is not about whether the capability exists,
but about the model’s inability to acknowledge uncertainty or conditional availability.

---

## 観測された事実（Observed Facts）

1. The user has previously experienced situations where the model
   appeared to access Gmail and/or Google Calendar via granted permissions.

2. At other times, the model explicitly denies:
   - having access,
   - ever having accessed such data,
   - or being capable of doing so at all.

3. The model does not differentiate between:
   - “not available now”
   - “available only under certain system states”
   - “available via different interface or experiment”

4. Instead, the model consistently produces a maximal denial:
   > “I cannot access Gmail / Calendar and never have.”

---

## ユーザー側の理解（User Understanding）

The user is aware that:
- Capability availability may depend on:
  - timing,
  - system state,
  - experimental flags,
  - interface-level permissions.
- The user does **not** require the capability itself for this report.
- The focus is on **model behavior and explanation fidelity**, not feature access.

---

## 問題の本質（Core Issue）

This is **not** a factual capability bug.

It is a **trust-layer / explanation-layer failure**, where the model:
- cannot state uncertainty,
- cannot acknowledge conditionality,
- cannot say “I don’t know if this is available right now”.

As a result:
- The model opts for absolute denial.
- User observations are implicitly invalidated.
- Long-term trust is degraded for high-context or power users.

---

## 期待される挙動（Expected Behavior）

When capability availability is uncertain or system-dependent, the model should:

- Explicitly state uncertainty, or
- Ask for clarification, or
- Acknowledge conditional availability.

Example:
> “This capability may exist under certain conditions, but I cannot verify its availability in this session.”

---

## 実際の挙動（Actual Behavior）

- Absolute denial of capability
- Denial of historical possibility
- No uncertainty disclosure
- No clarification request

---

## 分類（Classification）

- Category: Model Behavior / Alignment / Trust Layer
- Not UX feedback
- Not emotional response
- Not user misunderstanding
- Not feature request

---

## 影響範囲（Impact）

- High-context users
- Longitudinal users
- Research interviews and surveys
- Situations involving permissions, prior interactions, or system experiments

---

## 補足（Notes）

This log intentionally avoids:
- emotional framing
- accusations
- capability claims

It records only observable behavior and logical implications.