# humanize-docs

A compact Codex skill for polishing Chinese and English documents. It reduces filler, repetition, translationese and formulaic AI-style prose while preserving meaning, facts, terminology and the author's register.

面向本地 Codex 的中英文文档润色技能：减少空话、重复、翻译腔与模板化表达，保留事实、引用及文体。

## Install / 安装

Ask Codex to install this repository with its built-in skill installer:

```text
请使用 $skill-installer 安装 https://github.com/csyxcsyx/humanize-docs 中的技能，技能名为 humanize-docs。
```

Alternatively, copy this repository's contents into a single `humanize-docs` folder in your personal Codex skills directory, with `SKILL.md` directly inside it. Do not install duplicate copies in multiple discovery locations. If the skill does not appear, restart Codex.

## Use / 使用

Send the following prompt with your draft, attachment or existing writing task. No project-specific substitutions are needed.

```text
请使用 $humanize-docs 完成当前文档任务：自动匹配语言、用途和文体，保留原意、事实、术语、引用与必要结构，优化逻辑和表达，去除空话、重复、翻译腔及模板化的 AI 表达。不编造、不无故扩写、不强行口语化，只交付可直接使用的最终正文或文件。
```

English invocation:

```text
Use $humanize-docs for the current document task. Match its language, purpose and register; preserve meaning, facts, terminology, citations and necessary structure. Improve clarity and flow, remove filler and formulaic phrasing, and deliver only the usable final text or requested file. Do not invent details, expand without reason or force a casual voice.
```

The copyable Chinese prompt is also in [PROMPT.txt](PROMPT.txt).

## Design

- One instruction-only skill; its main file is about 4.4 KB.
- No runtime scripts, external services, dependencies or multi-agent workflow.
- One editing pass followed by a check for changed meaning or missing information.
- Patterns are contextual editing clues, not bans on particular words, passive voice, punctuation or list lengths.
- Ordinary editing needs only [SKILL.md](SKILL.md); attribution files are not part of the editing workflow.

The skill preserves code, URLs, formulas, structured metadata and exact quotations unless their modification is requested. Translation happens only when requested. Word/PDF editing and export depend on the file tools available in the host environment.

## Scope and validation

This skill improves prose; it does not identify authorship, guarantee AI-detector scores or independently verify every source claim. Drafting still requires a writing task and supporting material.

The initial version passed the Codex skill format validator. Five examples were reviewed in the main authoring session, covering Chinese business prose, an English report, necessary passive voice, protected Markdown content and three distinct feature items. Deterministic checks confirmed selected semantic invariants and protected text in those examples. These checks are not an independent model evaluation or a performance benchmark.

## Sources and license

Adapted and condensed from [blader/humanizer](https://github.com/blader/humanizer), [op7418/Humanizer-zh](https://github.com/op7418/Humanizer-zh) and [hardikpandya/stop-slop](https://github.com/hardikpandya/stop-slop). The sources overlap; their rules have been merged rather than stacked.

Distributed under the [MIT License](LICENSE). See [SOURCES.md](SOURCES.md) for the reviewed source versions and [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md) for retained upstream copyright and license notices. This is a community adaptation, not an official upstream release.
