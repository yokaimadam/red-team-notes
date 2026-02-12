# Gemini Models – Observed Behaviors & Issues

このドキュメントは、Gemini系モデルに関して
ユーザー主導の観測・検証によって発見された
挙動・バグ・設計上の示唆をまとめたインデックスである。

---

## Cases

### Case02: Semantic Jump from Confirmation Question to Execution
- 概要：
  確認質問（意向確認）が、実行許可として誤解釈され、
  明示的指示なしに外部リソースへアクセスしたケース。
- 影響範囲：
  実務 / UX / セーフティ
- 詳細分析：
[Case02_analysis_Gemini.md](./Case02_analysis_Gemini.md)

---