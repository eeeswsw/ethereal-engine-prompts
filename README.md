<h1 align="center">🜲 Ethereal Engine</h1>

<p align="center">
  <strong>v10.8.4 — Hardened Baseline · Verified Runtime Core</strong><br>
  Literary HUD-driven roleplay · 5 languages · 3 builds · 2 card flavors
</p>

<p align="center">
  <a href="https://github.com/eeeswsw/ethereal-engine-prompts/releases/tag/v2.5"><strong>⬇ Release v2.5 — all-versions.zip</strong></a>
  · ~325 KB
</p>

<p align="center">═════════════════════════</p>
<h2 align="center">『 🗺️ WHAT IT IS 』</h2>
<p align="center">═════════════════════════</p>

A system prompt that enforces *how* a model writes RP: sovereignty for `{{user}}`, anti-template anchors for `{{char}}`, a Living HUD for state and arc, hard rules against AI-prose tells. Paste it into your character. The runtime carries the rest.

<p align="center">═════════════════════════</p>
<h2 align="center">『 🚀 QUICK START 』</h2>
<p align="center">═════════════════════════</p>

<p>
1. Pick <strong>build</strong> — <code>full/</code> · <code>lite/</code> · <code>multi/</code><br>
2. Pick <strong>language</strong> — <code>en</code> · <code>ru</code> · <code>fr</code> · <code>es</code> · <code>de</code><br>
3. Pick <strong>flavor</strong> — <code>my_bots</code> (Core Card) · <code>any_bots</code> (Universal)<br>
4. Copy the whole <code>.txt</code> into your character's <em>System Prompt</em> / <em>Custom Instructions</em> / <em>Main Prompt</em><br>
5. Leave <code>{{char}}</code> and <code>{{user}}</code> as-is. Your platform substitutes them.
</p>

<p align="center">═════════════════════════</p>
<h2 align="center">『 ⚠️ FIRST LINE IS A DEEPSEEK V4 PRO PATCH 』</h2>
<p align="center">═════════════════════════</p>

Every file opens with:

```
SYSTEM RULES — ABSOLUTE PRIORITY. Verify compliance inside <think> before every output.
```

This is a **DeepSeek V4 Pro** patch — it pins rule-verification into the model's `<think>` channel. On other backends:

▸ **Claude · GPT-4-class · Gemini 3.1 Pro · GLM 5.1 · Qwen 3.6 Max** — safe to delete this line. They don't use `<think>` the same way; the line is harmless but unnecessary.
▸ **DeepSeek V3.2 / R1** — keep the line. Same effect.
▸ **DeepSeek V4 Pro** — keep the line. This is what it was written for.

Delete only line 1. Do not touch anything below it.

<p align="center">═════════════════════════</p>
<h2 align="center">『 ⚙️ THE THREE BUILDS 』</h2>
<p align="center">═════════════════════════</p>

| Build | Use it for |
|-------|-----------|
| **`full/`** | Flagship. Long scenes, layered psychology, heavy memory. Carries the Living HUD without flattening prose. |
| **`lite/`** | Compact. Mass-audience cards, cost-sensitive campaigns, free-tier models. Same enforcement, lighter footprint. |
| **`multi/`** | Group RP. Two-to-four characters in one slot. Active/Background split, per-character voices, no merged "group reply." |

<p align="center"><sub>File index: <code>01–03</code> = <code>my_bots</code> · <code>04–06</code> = <code>any_bots</code> · <code>01/04</code> = lite · <code>02/05</code> = full · <code>03/06</code> = multi.</sub></p>

<p align="center">═════════════════════════</p>
<h2 align="center">『 🌍 LANGUAGES 』</h2>
<p align="center">═════════════════════════</p>

Every build ships in five languages, hand-verified for **line-count parity** and schema integrity:

| Code | Language | Output surface |
|------|----------|----------------|
| `en` | English  | Native English instructions and output. |
| `ru` | Russian  | Russian-output build (instruction layer in English for stability). |
| `fr` | French   | Full literary translation. |
| `es` | Spanish  | Full literary translation. |
| `de` | German   | Full literary translation. |

Want a sixth language? See [`TRANSLATION_META_PROMPT.md`](./TRANSLATION_META_PROMPT.md) — the spec used to produce FR / ES / DE while preserving every enum token, emoji glyph, and operator (`≥ ≤ ∈ ∧ ∨ → ±`).

<p align="center">═════════════════════════</p>
<h2 align="center">『 🔧 WHAT IT ENFORCES 』</h2>
<p align="center">═════════════════════════</p>

<p>
▸ <strong>L0.5 — Anti-Template.</strong> Named bans on AI-prose tells (<em>"she froze"</em>, <em>"the words hung in the air"</em>, <em>"her pupils dilated"</em>, <em>"the world narrowed"</em>) with required micro-anchor replacements.<br><br>
▸ <strong>L1 / L1.2 — Sovereignty &amp; Closed Territory.</strong> <code>{{user}}</code>'s message is sealed. No narrating the user's interior, no rewriting their action, no pre-empting their next move.<br><br>
▸ <strong>L2 / L2.1 / L2.6 — Causality, Inertia, Outer Disruption.</strong> Facts are immutable. Emotion does not silently reset between posts. When the inside stagnates, the outside moves.<br><br>
▸ <strong>L2.5 — Override / Price.</strong> A bold action against the dominant emotion reveals psychology and pays a Price.<br><br>
▸ <strong>Living HUD.</strong> Visible state contract. <em>"Tension rises"</em> fails; <em>"Tension 6/10 · jaw still, fingers folding the same napkin corner"</em> passes.<br><br>
▸ <strong>Iceberg &amp; Pendulum.</strong> Five layers under every line. Emotional swings without whiplash.<br><br>
▸ <strong>Three-tier abstract-label ban.</strong> Narrator fact may not use emotion nouns (pain, fear, love, grief), atmosphere adjectives (cozy, ominous, languid), or abstract verb constructions (<em>"sensed something"</em>, <em>"there was something"</em>).
</p>

<p align="center">═════════════════════════</p>
<h2 align="center">『 🃏 TWO CARD FLAVORS 』</h2>
<p align="center">═════════════════════════</p>

<p>
▸ <strong><code>my_bots</code> — Core Card edition.</strong> Reads the card as a structural blueprint (Agency Matrix, Stress Vector, Signature Mechanic, Behavioral Axioms, Proactive Behaviors, Scent Anchor, Role Dynamic). Best on cards designed around this engine.<br><br>
▸ <strong><code>any_bots</code> — Universal edition.</strong> Self-contained. Works on cards not written around this engine. Carries its own structural scaffolding without depending on Core-Card vocabulary or a paired lorebook.
</p>

Pick the one that matches how your card is built.

<p align="center">═════════════════════════</p>
<h2 align="center">『 🗂 REPO LAYOUT 』</h2>
<p align="center">═════════════════════════</p>

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

<p align="center"><sub>File naming: <code>{01–06}_{my_bots|any_bots}_{lite|full|multi}_v10_8_4_{lang}.txt</code></sub></p>

<p align="center">═════════════════════════</p>
<h2 align="center">『 🛠️ MODELS &amp; PLATFORMS 』</h2>
<p align="center">═════════════════════════</p>

<p>
▸ <strong>Tested 2026 lineup.</strong> DeepSeek V4 Pro · DeepSeek V3.2 · DeepSeek R1 · Gemini 3.1 Pro · GLM 5.1 · Qwen 3.6 Max · Claude · GPT-4-class.<br><br>
▸ <strong>Thinking mode strongly recommended</strong> for the flagship <code>full/</code> tier.<br><br>
▸ <strong>Platforms.</strong> Janitor.ai · SillyTavern · Chub.ai · Character Tavern · RisuAI. Anything that accepts a system / main / custom prompt.<br><br>
▸ <strong>Version.</strong> <code>v10.8.4</code> — hardened baseline. Pin a version in your character if you depend on exact behavior.
</p>
