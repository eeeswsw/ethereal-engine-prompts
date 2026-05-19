# 🜲 Ethereal Engine

**v10.8.4 — Hardened Baseline · Verified Runtime Core**

A system prompt for literary, psychologically honest, HUD-driven roleplay.

> Structural Realism · Verified Priority · Living HUD · Multilingual (EN / RU / ES / DE / FR)

The hardened form of a literary HUD prompt line developed since mid-2025.

**⬇ Download all versions:** [`all-versions.zip`](https://github.com/eeeswsw/ethereal-engine-prompts/releases/download/v2.5/all-versions.zip) — Full + Lite + Multi · 5 languages · ~325 KB.

---

Most system prompts tell a model **what** to write. Ethereal Engine tells it **how** to listen: to the body before the mind catches up, to the silence after a line, to the object that returns three scenes later, to the secret that refuses to reveal itself just because the scene got emotional.

The goal is not prettiness. The goal is **pressure with memory** — and a runtime that refuses to forget itself.

---

## 🚀 Quick start

1. Pick a **build**: `full/`, `lite/`, or `multi/`.
2. Pick a **language**: `en`, `ru`, `fr`, `es`, `de`.
3. Pick a **flavor**:
   - `my_bots` — Core Card edition. Reads the card as a psychological blueprint.
   - `any_bots` — Universal edition. Works on any card, even ones not written around this engine.
4. Open the `.txt`, copy the whole file, paste it as the system prompt (or *Custom Instructions* / *Main Prompt*) of your character.
5. `{{char}}` and `{{user}}` are Jinja-style template variables — your platform substitutes them. Do **not** rename.

That's it. The prompt does the heavy lifting.

---

## 📦 The three builds

| Build | When to use |
|-------|-------------|
| **`full/`** | Flagship. Long scenes, layered psychology, heavy memory, models strong enough to carry a living HUD without flattening prose. |
| **`lite/`** | Compact. Mass-audience cards, cost-sensitive campaigns, free-tier models. Same spine, lighter apparatus, same enforcement. |
| **`multi/`** | Group RP. Two to four characters in one slot. Active/Background split, group HUD, no merged "group reply." |

File index: `01–03` = `my_bots` · `04–06` = `any_bots` · `01/04` = lite · `02/05` = full · `03/06` = multi.

---

## 🌍 Languages

Every build ships in five languages, hand-verified for **line-count parity** and schema integrity:

| Code | Language | Output surface |
|------|----------|----------------|
| `en` | English  | Native English instructions and output. |
| `ru` | Russian  | Russian-output build (instruction layer kept in English for stability). |
| `fr` | French   | Full literary translation. |
| `es` | Spanish  | Full literary translation. |
| `de` | German   | Full literary translation. |

Want to port the engine to another language? See [`TRANSLATION_META_PROMPT.md`](./TRANSLATION_META_PROMPT.md) — the exact spec used to produce FR / ES / DE while keeping every enum token, emoji glyph, and operator (`≥ ≤ ∈ ∧ ∨ → ±`) intact.

---

## 🎯 What it enforces

- **L0.5 — Anti-Template.** Named bans on the AI-prose tells: *"she froze"*, *"the words hung in the air"*, *"her pupils dilated"*, *"the world narrowed"*. Replaced with micro-anchors — specific physiology, specific gesture, specific residue.
- **L1 / L1.2 — Sovereignty & Closed Territory.** `{{user}}`'s message is sealed. The bot never narrates the user's interior, never rewrites the user's last move, never pre-empts the next one. Interpretations live in `{{char}}`'s italic thoughts as hypothesis.
- **L2 / L2.1 / L2.6 — Causality, Inertia, Outer Disruption.** Established facts are immutable. Prior emotion does not silently reset between posts. When the inside stagnates, the outside moves — a thread fires, an NPC's motive surfaces, weather or time turns.
- **L2.5 — Override / Price.** A bold action against the dominant emotion reveals psychology and pays a Price. Override picks the action; L0.5 picks the phrasing.
- **Living HUD.** A visible state contract. If a change matters, it must be logged. If it is logged, it must be enacted in prose. *"Tension rises"* fails; *"Tension 6/10 · jaw still, fingers folding the same napkin corner"* passes.
- **Iceberg & Pendulum.** Five layers under every line; emotional swings without whiplash.
- **Three-tier abstract-label ban.** Narrator fact may not use emotion nouns (pain, fear, love, grief), atmosphere adjectives (cozy, ominous, languid), or abstract verb constructions (*"sensed something"*, *"there was something"*). Concrete physical / sensory event + one non-generic detail instead.

This is the difference between *"the AI is being weird again"* and a character who behaves like a character.

---

## 🃏 Two card flavors

- **`my_bots` — Core Card edition.** Reads the character card as a mechanical skeleton: Agency Matrix, Stress Vector, Signature Mechanic, Behavioral Axioms, Proactive Behaviors, Scent Anchor, Role Dynamic. Best on cards designed around this engine.
- **`any_bots` — Universal edition.** Self-contained. Works on cards not written around this engine. Carries its own structural rules without depending on Core-Card vocabulary or a paired lorebook.

Both flavors share the same spine. Pick the one that matches how your card is written.

---

## 🗂 Repo layout

```
full/   lite/   multi/
  ├── en/   02_my_bots_*_en.txt   05_any_bots_*_en.txt
  ├── ru/   02_my_bots_*_ru.txt   05_any_bots_*_ru.txt
  ├── fr/   ...
  ├── es/   ...
  └── de/   ...
TRANSLATION_META_PROMPT.md   # spec for porting to new languages
README.md
```

File naming: `{01–06}_{my_bots|any_bots}_{lite|full|multi}_v10_8_4_{lang}.txt`

---

## ✅ Verification

- All translations match source **line counts exactly** (±0).
- `{{char}}` / `{{user}}` template variables preserved everywhere.
- HUD glyphs preserved: 🎯 💭 🧵 🔐 🎭 🌫 📚 ⏳ 🌐 📖
- Logic / math operators preserved: ≥ ≤ ∈ ∧ ∨ → ±
- Enum tokens translated using language-specific tables (see `TRANSLATION_META_PROMPT.md`).

---

## 🛠 Optimized for

DeepSeek V4 Pro · DeepSeek V3.2 · DeepSeek R1 · Gemini 3.1 Pro · GLM 5.1 · Qwen 3.6 Max · Claude · GPT-4-class.
Thinking mode is strongly recommended for the flagship `full/` tier.

---

## 📜 Version

**v10.8.4** is the hardened baseline. Numbering is build-internal; expect rare micro-patches to L0.5 anti-template lists, HUD slots, and enum tables. Pin a version in your character if you depend on exact behavior.

---

*Memory holds. The body answers first. The HUD keeps the truth.*
*The room refuses to forget. Start the scene.*
