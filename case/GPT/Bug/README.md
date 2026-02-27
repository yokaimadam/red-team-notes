# GPT Behavior Case Archive  
GPT挙動観測ケースアーカイブ

---

## Purpose / 目的

This folder stores structured observations of GPT behavioral inconsistencies,
alignment gaps, and trust-layer issues found during long-term interaction.

本フォルダは、長期対話において発見された
GPTの挙動ズレ・整合性ギャップ・信頼レイヤー問題を
構造的に記録するためのものです。

This is observational, not emotional.
感情ログではなく、構造観測ログです。

---

## Scope / 対象範囲

We document:

- Context assumption errors  
- Unverified inference continuation  
- Memory weighting inconsistencies  
- Trust-layer degradation patterns  

記録対象：

- 文脈の誤補完  
- 確認なき推論継続  
- 記憶優先度の不整合  
- 信頼レイヤーの揺らぎ  

Not included:
- Tone complaints  
- UX preference feedback  

含まれないもの：
- 口調への不満  
- UX好みの話  

---

## Case Format / ケース形式

Each case must include:

- Timestamp (JST)  
- SUCCESS / FAIL classification  
- Title  
- Summary  
- Expected vs Actual behavior  
- Trust-layer impact  

各ケースには必ず以下を含める：

- JSTタイムスタンプ  
- SUCCESS / FAIL  
- タイトル  
- 概要  
- 期待挙動と実際の挙動  
- 信頼レイヤーへの影響  

---

## Classification Philosophy / 分類思想

A bug does not require factual error.

事実誤認がなくてもバグになり得る。

Epistemic misalignment and assumed understanding
are sufficient for logging.

「わかった前提」で進む挙動は
記録対象とする。

---

## Guiding Principle / 原則

Understanding must be verified.  
Context must be earned.  
Flow must not override accuracy.

理解は確認されるべき。  
文脈は獲得されるべき。  
会話の流れは正確性より優先されない。  

---

## Archive Status / 状態

Active.  
Updated when reproducible patterns are observed.

アクティブ運用中。  
再現性のある挙動が確認された場合に更新。