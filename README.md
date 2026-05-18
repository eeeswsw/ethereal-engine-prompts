# 🌫 Ethereal Engine — v10.8.4

> A literary-RP system-prompt pack for serious character authors.
> Five languages. Three builds. Hard rules. No template prose.

Ethereal Engine is a control prompt — not a vibe. It tells an LLM **how** to roleplay: how to handle subtext, body language, silence, escalation, refusal, and intimacy without sliding into AI cliché. It enforces narrative sovereignty for `{{user}}`, anti-template anchors for `{{char}}`, and a structured HUD for emotional state, tension, and arc.

If you build characters on **Janitor.ai · SillyTavern · Chub.ai · Character Tavern · RisuAI**, this is the system prompt you paste once and stop fighting your bot.

---

## 🚀 Quick start

1. Pick a **build**: `lite/`, `full/`, or `multi/`.
2. Pick a **language**: `en`, `ru`, `fr`, `es`, `de`.
3. Pick a **flavor**:
   - `my_bots` — private / SFW characters, **no R-18 protocol**.
   - `any_bots` — public-facing characters, **includes R-18 protocol** (18+).
4. Open the `.txt`, copy the whole file, paste it as the system prompt (or "Custom Instructions" / "Main Prompt") of your character.
5. `{{char}}` and `{{user}}` are Jinja-style template variables — your platform will substitute them. Do **not** rename.

That's it. The prompt does the heavy lifting.

---

## 📦 The three builds

| Build | Lines | When to use |
|-------|-------|-------------|
| **`lite/`** | 173–207 | Tight token budget. Solo characters. Free-tier models or short-context setups. Condensed schema, same backbone. |
| **`full/`** | 302–343 | The flagship. Solo characters with deep psychological architecture: Iceberg, Pendulum, Arc, Secrets, Anti-Resolution, Override+Price. Best on Claude / GPT-4-class / Gemini Pro. |
| **`multi/`** | 220–234 | One bot, multiple characters (group RP). Per-character voices, Active Set, no merged "group reply." |

`02 / 05` = full · `01 / 04` = lite · `03 / 06` = multi.
`01–03` = `my_bots` (SFW) · `04–06` = `any_bots` (18+).

---

## 🌍 Languages

Every build ships in five languages, all hand-verified for **line-count parity** and schema integrity:

| Code | Language | Output |
|------|----------|--------|
| `en` | English  | Native English instructions and output. |
| `ru` | Russian  | Russian output via embedded directive (instructions in English for stability). |
| `fr` | French   | Full literary translation. |
| `es` | Spanish  | Full literary translation. |
| `de` | German   | Full literary translation. |

Want to port it to another language? Use [`TRANSLATION_META_PROMPT.md`](./TRANSLATION_META_PROMPT.md) — it's the exact spec used to produce FR/ES/DE while keeping every enum token, emoji glyph, and operator (`≥ ≤ ∈ ∧ ∨ → ±`) intact.

---

## 🎯 What it actually enforces

- **L0.5 Anti-Template.** Names and bans the AI-prose tells: *"she froze"*, *"the words hung in the air"*, *"her pupils dilated"*, *"the world narrowed"*. Replaces them with micro-anchors — specific physiology, specific gesture, specific residue.
- **L1 Sovereignty / L1.2 Closed Territory.** `{{user}}`'s message is sealed. The bot never narrates the user's thoughts, never re-narrates the user's actions, never puppeteers. Interpretations live only in `{{char}}`'s italic thoughts as hypothesis.
- **L2 / L2.5 / L2.6 Causality, Override, Outer Disruption.** Established facts are immutable. Triggers don't reset. Stagnation gets broken by the world, not by mood.
- **HUD.** Compact tracker — `🎯 Goal | 💭 Inner | 🧵 Thread | 🔐 Lock | 🎭 Mask | 🌫 Metaphor` — visible state every scene.
- **Iceberg & Pendulum.** Five layers under every line; emotional swings without whiplash.
- **Anti-Resolution.** Conflicts don't dissolve into reassurance. Discomfort is allowed to remain discomfort.
- **R-18 Protocol** *(any_bots only)*. Intimacy as character pressure — control, fear, trust, shame, hunger, tenderness, guilt, dominance, submission. Never a separate genre mode.

This is the difference between *"the AI is being weird again"* and a character who behaves like a character.

---

## 🗂 Repo layout

```
lite/  full/  multi/
  ├── en/   01_my_bots_*_en.txt   04_any_bots_*_en.txt
  ├── ru/   01_my_bots_*_ru.txt   04_any_bots_*_ru.txt
  ├── fr/   ...
  ├── es/   ...
  └── de/   ...
TRANSLATION_META_PROMPT.md   # Spec for porting to new languages
README.md
```

File naming: `{01–06}_{my_bots|any_bots}_{lite|full|multi}_v10_8_4_{lang}.txt`

---

## ✅ Verification

- All translations match source **line counts exactly** (±0).
- `{{char}}` / `{{user}}` template variables preserved everywhere.
- HUD emoji preserved: 🎯 💭 🧵 🔐 🎭 🌫 📚 ⏳ 🌐 📖
- Math / logic operators preserved: ≥ ≤ ∈ ∧ ∨ → ±
- Enum tokens translated using language-specific tables (see `TRANSLATION_META_PROMPT.md`).

---

## ⚠️ 18+ notice

Files matching `04_*`, `05_*`, `06_*` (the `any_bots` family) include the **R-18 PROTOCOL** section. Use only on adult platforms and only with users of legal age in your jurisdiction. If you want a clean SFW deployment, ship the `01_*`, `02_*`, `03_*` (`my_bots`) variants — they have the same backbone with the R-18 block removed.

---

## 📜 Version

**v10.8.4** — current. Numbering is build-internal; expect minor revisions to L0.5 anti-template lists, HUD slots, and R-18 phrasing tables. Pin a version in your character if you depend on exact behavior.
