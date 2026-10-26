# Sources and adaptation

Reviewed: 2026-10-24 (Asia/Shanghai). Stars are GitHub repository totals observed during this task, not skill-level ratings or proof of quality. This is a local adaptation, not an official upstream release.

- [blader/humanizer](https://github.com/blader/humanizer): 60,132 stars; MIT. Role: 英文 AI 写作模式、作者声音、事实与文件保护.
  - Observed main HEAD: `8c307f367c91bd974002f10f2be2965d642c13df`.
  - Reviewed SKILL.md blob: `19fc634208e8cc6ae55d4ff287152583216fd244`.
- [op7418/Humanizer-zh](https://github.com/op7418/Humanizer-zh): 20,574 stars; MIT. Role: 中文句法、翻译腔、四字词堆叠及语义边界.
  - Observed main HEAD: `f4518a8eab97b8bfebc66a89d34320a89bef6930`.
  - Reviewed SKILL.md blob: `ef07b54da21a41d4a7e4fe0b0afb928f597eb684`.
- [hardikpandya/stop-slop](https://github.com/hardikpandya/stop-slop): 18,289 stars; MIT. Role: 删冗、直接表达、句子节奏与信息密度.
  - Observed main HEAD: `8da1f030185bdfe8471220585162991eaeb970e9`.
  - Reviewed SKILL.md blob: `83f2032fde406e97492ec48ee05ebe46f6403109`.

## Adaptation decisions

Merged overlapping rules into one instruction-only entry point. Kept factual fidelity, register matching, Chinese/English editing and a single final meaning check. Removed exhaustive pattern catalogs, long examples, scoring thresholds, mandatory draft/critique outputs, absolute bans on adverbs/passives/dashes and fixed list lengths. No executable upstream scripts, network dependencies, hooks, agents or configuration changes are included.

The Chinese project derives partly from the English project and references Stop Slop; these are related sources, not three independent evaluations. Treat patterns as editing heuristics, not an authorship test. No detector-evasion, accuracy, speed or token-saving percentage is promised.

## Provenance access

SOURCES.md and THIRD_PARTY_NOTICES.md are attribution records. They are not required during ordinary writing. The package contains the adapted instructions and retained upstream notices; it does not include upstream runtime scripts.

