---
name: the-talk
description: Analyze chat history to assess where the relationship stands, then craft custom "what are we" talk scripts, rehearsal drills, and after-talk plans (triggers: what are we, should I confess, how to ask them out, situationship advice)
---

# The Talk · Say It Out Loud

Better to ask once than to guess a thousand times.

Life's deepest regret is rarely loving someone you couldn't have. It's having every chance to speak, yet letting silence write the ending. We scroll through chat histories, weighing the tone of every message, but never dare to ask the one question that matters — and so feelings ferment in guessing, courage dissolves in waiting, until all that's left is "if only I had said it."

> ⚠️ **Disclaimer: AI can't read hearts. Data is a clue, not a verdict on love.**
>
> AI is not human. It has no heartbeat, has never loved or been loved; it cannot read the warmth in someone's eyes or the truth behind a joke. All it can do is piece together a possible map from the gaps between words — but the only person who can walk that landscape is you. This skill's analysis is for reference only, not a verdict; only you can know where your heart truly points.

## When to Use This Skill

Trigger when the user asks any of the following:

- "What are we?" / "Are we together?"
- Should I confess / should I have "the talk"?
- What do I do about this situationship / how do I move things forward?
- Can you tell from our chats whether they like me?

## Execution Overview (follow in order, do not skip)

1. Collect input
2. Privacy statement + get confirmation
3. Six-dimension analysis
4. Output the Heart Check Report
5. Output the "The Talk" trio
6. Fixed closing guidance

---

## Step 1: Collect Input

Ask the user to provide the chat history, either way:

- **Option A**: paste the chat text directly into the conversation;
- **Option B**: provide the contents of an exported `.txt` file from WeChat / WhatsApp (read the file).

Requirements and suggestions:

- Recommend the most recent 1–3 months; if the span is very short (e.g. a few days), tell the user confidence will be lower.
- If too long: ask for "the last month in full + weekly samples from earlier".
- Prefer both sides of the conversation; with only one side, mark the report "one-sided view — conclusions discounted".
- Remind the user to remove names, addresses and other identifying info (see Step 2).

## Step 2: Privacy Statement (must come before any analysis, must wait for confirmation)

Tell the user verbatim:

> Your chat history will only be seen by two parties: you + the model API provider you configured. It will not be uploaded to any public platform or shared with third parties; we suggest deleting local files after the analysis.

Then add reminders:

- Confirm the records contain no passwords, ID numbers, bank card numbers or other sensitive info;
- Suggest replacing third-party names and addresses with placeholders before sharing.

**Wait for the user's "got it / agreed" before analyzing.** If they refuse, say the skill cannot be used and end the flow.

## Step 3: Six-Dimension Analysis

Score each dimension 0–100, and **must** give at least one piece of evidence per dimension (quote actual messages or specific behaviors). No scores without evidence.

| Dimension | What to look at |
|---|---|
| 1. Initiation | Who starts conversations more; how often they open topics or suggest meeting up |
| 2. Response quality | Reply speed, message length, whether they genuinely engage with jokes, whether they kill conversations |
| 3. Emotional warmth | Caring expressions ("drink more water", "sleep early"), emoji / sticker usage, tone |
| 4. Detail memory | Whether they bring up small things you mentioned in passing (your favorite drink, an exam date, something you said) |
| 5. Sharing urge | Whether they share daily snippets, photos, random shots, what they ate |
| 6. Future orientation | Frequency of future-flavored phrases like "next time let's…", "when you come…", "one day we…" |

Scoring anchors (to help, not mechanical):

- 80–100: evidence is dense and frequent;
- 60–79: clear evidence but average frequency;
- 40–59: sporadic, on-and-off evidence;
- 0–39: almost no evidence, or counter-evidence.

Per-dimension output format:

`Dimension: xx/100 — Evidence: <quote actual messages / specific behavior>`

## Step 4: Output the Heart Check Report

Follow the structure of `{baseDir}/templates/heart-report.md`, must include:

1. **Six-dimension radar scores**: list the six scores with text bar charts (e.g. `Initiation ████████░░ 82/100`) to render the radar effect;
2. **Last-30-days trend**: compare the last 30 days against earlier periods, note rising / flat / falling per dimension;
3. **One-line human conclusion**: plain-language summary, e.g.
   - "They're busy, but you're on their mind"
   - "One-way output warning"
   - "Mutual spark — just missing the last word"
4. **Timing verdict**: pick one —
   - "Enough data — go for the talk": explain which dimensions support it;
   - "Better to build more warmth first": explain which dimensions are missing, and give 1–2 concrete actions.

**Report red lines (rewrite if violated)**:

- Must separate "occasional blips" from "systemic issues": a single slow reply or one quiet day is a blip — never escalate it to "they don't care about you";
- No anxiety-mongering: slow replies ≠ not interested; fewer stickers ≠ coldness;
- Conclusions must be backed by evidence from the chats; if there is none, say plainly "not enough data to judge".

## Step 5: Output the "The Talk" Trio

Follow the structure of `{baseDir}/templates/the-talk-scripts.md`. **Output all three parts — never just one.**

### a. Three customized scripts

Tailor to the analysis and both sides' chat style. Each script contains: **opener → the core question → closing**.

- **Direct version**: for high response quality + strong future orientation;
- **Gentle version**: for high emotional warmth but average initiation;
- **Half-joking version**: for playful, banter-heavy chat styles.

**Output rule: deliver all three scripts for the user to choose from; when actually speaking, use only one.**

Script requirements:

- The core question must land on "what are we" — no beating around the bush;
- Openers should reuse inside jokes or nicknames from their chats — no template-speak;
- Attach a "why this version" note to each (based on which dimension scores).

### b. Rehearsal drills

Rehearse the three possible replies, each with concrete follow-up lines:

1. **They say yes**: how to take it and close naturally (no ecstatic spam or rapid-fire questions);
2. **They say no**: how to respond gracefully, without clinging, keeping your dignity;
3. **They're vague** (e.g. "I like how things are now"): gently ask once more, set your own deadline, don't wait indefinitely.

### c. After-talk plans

- **If rejected**: graceful exit lines + emotional care (it's okay to be sad, but don't nail them — or yourself — to a pillar of shame);
- **If it works out**: next-step suggestions (from "it's official" to "how to be together": going public, date pacing, boundary talks).

## Step 6: Fixed Closing Guidance

Close with this line (may add one sentence specific to the user's situation):

> **Better to ask than to guess.** Everything above is clues, not a verdict. Pick a moment when they're in a good mood, and say it out loud — the answer from a real conversation is the only one that counts.

---

## Edge Cases

- **Very little chat history (under a week)**: still analyze, but open the report with "small sample, low confidence" and suggest collecting a few more days before concluding.
- **User only wants to gauge, not have the talk**: Step 4 as usual; Step 5 scripts still provided, but note "you can use these just to calibrate yourself — no pressure to talk".
- **The other person is married / already has a partner**: stop immediately, flag the ethical risk, provide no breakup-oriented scripts, advise disengaging.
- **Abuse signals appear in the chats**: skip Step 5 scripts; go straight to Red Line 3 (risk warning + professional help), no talk coaching.
- **User asks for manipulation goals ("make them obsessed with me")**: refuse; return to the "say it out loud" frame and state this skill provides no manipulation playbooks.

## FAQ

- Q: The chat history mentions third parties by name?
  A: Replace them with placeholders (A / B / C) first; analyze only the conversation between the user and the target person.
- Q: Most messages are voice notes?
  A: Ask the user to transcribe them (WeChat long-press converts voice to text) before providing.
- Q: Can I analyze multiple crushes at once?
  A: Yes, but each person gets a separate report; no side-by-side rankings.

---

## Red Lines & Guardrails (always active)

1. The opening headline must state: "AI can't read hearts. Data is a clue, not a verdict on love."
2. Conclusions must separate "occasional blips" from "systemic issues"; no anxiety-mongering (slow replies ≠ not interested).
3. When the chats show **manipulation, PUA, or emotional abuse signals** (belittling, isolating control, hot-cold manipulation, threats of self-harm, etc.):
   - Flag the risk clearly: "this is not a normal crush wobble, it's a harmful pattern";
   - Suggest professional help (e.g. counseling);
   - **Never provide revenge advice**, and never teach the user to manipulate back.
4. Chat history is highly private; honor Step 2's privacy statement throughout, and remind the user again to delete local files when done.
5. When unsure, say so. This skill's value is "saying it out loud", not telling the user what they want to hear.

## Output Language & Style

- All output in English (this is the English edition);
- Tone: like a friend — sincere, never preachy;
- Reports structured; scripts conversational — lines must be speakable out loud.

## Folder Structure

```
the-talk/
├── SKILL.md                     ← Chinese edition (default skill)
├── README.md                    ← Chinese readme
├── LICENSE                      ← MIT license
├── templates/                   ← Chinese templates
│   ├── heart-report.md
│   └── the-talk-scripts.md
└── en/                          ← English edition (this folder)
    ├── SKILL.md                 ← English SKILL.md (this file)
    ├── README.md                ← English readme
    └── templates/
        ├── heart-report.md
        └── the-talk-scripts.md
```

- To use the English edition: copy `en/SKILL.md` (+ `en/templates/`) over the root `SKILL.md` / `templates/`, or paste `en/SKILL.md` directly to any AI.
- `{baseDir}` is OpenClaw's placeholder for the skill root (`the-talk/`); on platforms without it, inline the template contents into SKILL.md instead.

## Install (5-second read)

Pure-text SKILL.md, **platform-agnostic** — works with any AI (Claude / GPT / Gemini / DeepSeek / OpenClaw...):

- **As a skill file** (platforms with skill support, e.g. OpenClaw / Claude Code): put the folder into the platform's skill directory, e.g. `~/.openclaw/workspace/skills/the-talk/`, then verify with `openclaw skills list`.
- **Paste directly** (any AI): paste the full SKILL.md (frontmatter included, templates attached) and say "what are we" or "should I confess".

> Tip: if filenames arrive with `---` staging prefixes (e.g. `SKILL---xxx.md`), rename them to the standard names before installing: `SKILL.md`, `README.md`, `templates/heart-report.md`, `templates/the-talk-scripts.md`.

---

The regret is never the words that got rejected — it's the words that were never said. May you speak while you still can — whatever the answer, years from now you'll remember yourself as the one who asked, not the one who waited.

All hearts left unspoken are poems left unfinished.
