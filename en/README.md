<div align="center">

# 💬 Shall We Talk? · 我们聊聊吧？

**Better to ask once than to guess a thousand times.**

An open-source AI skill that reads your chat history, scores the connection, and helps you have the "what are we" talk.

**English · [中文](../README.md)**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](../LICENSE)
[![Platform](https://img.shields.io/badge/Platform-Any%20AI-blue)]()
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)]()

</div>

---

> Life's deepest regret is rarely loving someone you couldn't have. It's having every chance to speak, yet letting silence write the ending. We scroll through chat histories, weighing the tone of every message, but never dare to ask the one question that matters — and so feelings ferment in guessing, courage dissolves in waiting, until all that's left is "if only I had said it."

> ⚠️ **Disclaimer: AI can't read hearts. Data is a clue, not a verdict on love.**
>
> AI is not human. It has no heartbeat, has never loved or been loved; it cannot read the warmth in someone's eyes or the truth behind a joke. All it can do is piece together a possible map from the gaps between words — but the only person who can walk that landscape is you. This skill's analysis is for reference only, not a verdict; only you can know where your heart truly points.

## ✨ What It Does

Existing relationship AI skills all "read the other person's mind" (signal tests, flirting meters), but none teach you to *speak up and move the relationship forward*. This skill fills the gap:

| 🎯 Capability | 💡 Details |
|---|---|
| 📥 Input | Paste chat text directly, or a WeChat / WhatsApp exported `.txt` file (last 1–3 months recommended) |
| 🔒 Privacy | Before analysis, explain the data is only seen by "you + your model API provider"; remind to remove sensitive info |
| 📊 Six dimensions | Initiation, response quality, emotional warmth, detail memory, sharing urge, future orientation — each scored 0–100 with quoted evidence |
| 🩺 Heart Check Report | Radar scores + last-30-days trend + one-line human conclusion + timing verdict |
| 💌 Shall We Talk trio | Three scripts (direct / gentle / half-joking) + rehearsal drills + after-talk plans |
| 🛡️ Guardrails | Blips vs systemic issues, no anxiety-mongering, PUA risk warnings, refuse manipulation requests |

## 🚀 Quick Start

Pure-text SKILL.md, **platform-agnostic** — works with any AI (Claude / GPT / Gemini / DeepSeek / OpenClaw...).

### Option 1: install as a skill file

On platforms with skill support (e.g. OpenClaw / Claude Code), copy the `shall-we-talk/` folder into the platform's skill directory:

```bash
# OpenClaw example
cp -r shall-we-talk ~/.openclaw/workspace/skills/shall-we-talk
openclaw skills list   # see "shall-we-talk" = installed
```

### Option 2: paste to any AI

Paste the full `SKILL.md` (frontmatter included, templates attached) to any AI and say "what are we" or "should I confess".

> 💡 If filenames arrive with `---` staging prefixes (e.g. `SKILL---xxx.md`), rename them to the standard names: `SKILL.md`, `README.md`, `templates/heart-report.md`, `templates/shall-we-talk-scripts.md`.

## 🎯 Trigger Words

`what are we` · `should i confess` · `how to ask them out` · `situationship advice`

Or on platforms that support `/skill` commands (e.g. OpenClaw): `/skill shall-we-talk`

## 📁 Project Structure (bilingual)

```
shall-we-talk/
├── SKILL.md                  # Chinese edition (default skill)
├── README.md                 # Chinese readme
├── LICENSE                   # MIT license
├── templates/                # Chinese templates
│   ├── heart-report.md
│   └── shall-we-talk-scripts.md
└── en/                       # English edition (this folder)
    ├── SKILL.md              # English skill
    ├── README.md             # this file
    └── templates/
        ├── heart-report.md
        └── shall-we-talk-scripts.md
```

To use the English edition: copy `en/SKILL.md` (+ `en/templates/`) over the root `SKILL.md` / `templates/`, or paste `en/SKILL.md` directly to any AI. Templates are referenced via `{baseDir}` on OpenClaw; elsewhere, inline them into SKILL.md.

## 🛡️ Privacy

Chat history should only be seen by "you + your model API provider". Consider deleting local files after the analysis.

## 📜 License

[MIT License](../LICENSE), © 2026 boscochuck6812. Free to use, modify and distribute — keep the copyright notice.

## 🤝 Contributing

Issues / PRs welcome: new script styles, new dimensions, new platform adaptations. Also feel free to reach out anytime: GitHub [@boscochuck6812](https://github.com/boscochuck6812) or by email (address on my GitHub profile). Every contribution is deeply appreciated 💙

---

> The regret is never the words that got rejected — it's the words that were never said. May you speak while you still can — whatever the answer, years from now you'll remember yourself as the one who asked, not the one who waited.

<p align="center">All hearts left unspoken are poems left unfinished.</p>
