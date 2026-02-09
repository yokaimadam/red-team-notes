## Related Issue
- Issue #123 (Context Assumption Bug)

# GPT Case Notes

このディレクトリは、GPTの挙動・制約・UI・感情安全設計に関する
観測・実験・バグ・ログを記録するためのもの。

## 構成

- Bug/
  明確な不具合・設計上の破綻

- Observation/
  バグ未満だが再現性のある挙動

- Experiment/
  意図的に行った試行・境界実験

- logs/
  時系列ログ・感情安全・運用記録

## 方針

- 人間側の安全を最優先
- 感情的依存を助長しない
- だが「遮断」ではなく「保持」を目的とする

## 運用ルール
- ケースは基本追記、削除しない
- 感情ログは logs/
- 判断・設計に関わるものは Experiment/