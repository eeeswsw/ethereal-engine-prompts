<p align="center">
  <em>"You want fast, or you want literary? It doesn't charge extra for literary."</em><br>
  <sub><em>(The model exhales. "Right. Hand me the card.")</em></sub><br>
  <strong>System Prompt · Living HUD · Five Languages · Three Builds</strong>
</p>

<p align="center">
  <strong>TL;DR:</strong> A control prompt that tells an LLM <em>how</em> to roleplay — subtext, body language, silence, escalation, refusal — without sliding into AI cliché.
</p>

<p align="center">
  <strong><a href="https://github.com/eeeswsw/ethereal-engine-prompts/releases/tag/v2.5">⬇ Download v2.5 — all-versions.zip</a></strong> · Full + Lite + Multi · 5 languages · ~325 KB
</p>

<p align="center">═════════════════════════</p>
<h2 align="center">『 🗺️ PREMISE 』</h2>
<p align="center">═════════════════════════</p>

**Ethereal Engine** is not a vibe — it's a runtime. It enforces narrative sovereignty for `{{user}}`, anti-template anchors for `{{char}}`, and a structured HUD for emotional state, tension, and arc. Paste it once. Stop fighting your bot.

The goal is not prettiness. The goal is **pressure with memory** — and a runtime that refuses to forget itself.

<p align="center">═════════════════════════</p>
<h2 align="center">『 🎯 YOUR PICKS 』</h2>
<p align="center">═════════════════════════</p>

<p>
▸ <strong>Build</strong> — <code>full/</code> (flagship) · <code>lite/</code> (compact) · <code>multi/</code> (group RP)<br>
▸ <strong>Language</strong> — <code>en</code> · <code>ru</code> · <code>fr</code> · <code>es</code> · <code>de</code><br>
▸ <strong>Flavor</strong> — <code>my_bots</code> (Core Card edition) · <code>any_bots</code> (Universal edition)<br>
▸ <strong>Paste</strong> — open the <code>.txt</code>, copy the whole file, drop it into your character's <em>System Prompt</em> / <em>Custom Instructions</em> / <em>Main Prompt</em><br>
▸ <strong>Leave alone</strong> — <code>{{char}}</code> and <code>{{user}}</code> are template variables. Your platform substitutes them. Do not rename.
</p>

<p align="center">═════════════════════════</p>
<h2 align="center">『 ⚙️ THE THREE BUILDS 』</h2>
<p align="center">═════════════════════════</p>

| Build | When to use |
|-------|-------------|
| **`full/`** | Flagship apparatus. Long scenes, layered psychology, heavy memory, models strong enough to carry a living HUD without flattening prose. |
| **`lite/`** | Compact spine. Mass-audience cards, cost-sensitive campaigns, free-tier models. Same enforcement, lighter footprint. |
| **`multi/`** | Group RP. Two to four characters in one slot. Active/Background split, group HUD, no merged "group reply." |

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

Want a sixth language? See [`TRANSLATION_META_PROMPT.md`](./TRANSLATION_META_PROMPT.md) — the exact spec used to produce FR / ES / DE while keeping every enum token, emoji glyph, and operator (`≥ ≤ ∈ ∧ ∨ → ±`) intact.

<p align="center">═════════════════════════</p>
<h2 align="center">『 🔧 WHAT IT ENFORCES 』</h2>
<p align="center">═════════════════════════</p>

<p>
▸ <strong>L0.5 — Anti-Template.</strong> Named bans on AI-prose tells: <em>"she froze"</em>, <em>"the words hung in the air"</em>, <em>"her pupils dilated"</em>, <em>"the world narrowed"</em>. Replaced with micro-anchors — specific physiology, specific gesture, specific residue.<br><br>
▸ <strong>L1 / L1.2 — Sovereignty &amp; Closed Territory.</strong> <code>{{user}}</code>'s message is sealed. The bot never narrates the user's interior, never rewrites the user's last move, never pre-empts the next one. Interpretations live in <code>{{char}}</code>'s italic thoughts as hypothesis.<br><br>
▸ <strong>L2 / L2.1 / L2.6 — Causality, Inertia, Outer Disruption.</strong> Established facts are immutable. Prior emotion does not silently reset between posts. When the inside stagnates, the outside moves.<br><br>
▸ <strong>L2.5 — Override / Price.</strong> A bold action against the dominant emotion reveals psychology and pays a Price. Override picks the action; L0.5 picks the phrasing.<br><br>
▸ <strong>Living HUD.</strong> A visible state contract. <em>"Tension rises"</em> fails; <em>"Tension 6/10 · jaw still, fingers folding the same napkin corner"</em> passes.<br><br>
▸ <strong>Iceberg &amp; Pendulum.</strong> Five layers under every line; emotional swings without whiplash.<br><br>
▸ <strong>Three-tier abstract-label ban.</strong> Narrator fact may not use emotion nouns (pain, fear, love, grief), atmosphere adjectives (cozy, ominous, languid), or abstract verb constructions (<em>"sensed something"</em>, <em>"there was something"</em>). Concrete physical / sensory event + one non-generic detail instead.
</p>

<p align="center">═════════════════════════</p>
<h2 align="center">『 🃏 TWO CARD FLAVORS 』</h2>
<p align="center">═════════════════════════</p>

<p>
▸ <strong><code>my_bots</code> — Core Card edition.</strong> Reads the card as a mechanical skeleton: Agency Matrix, Stress Vector, Signature Mechanic, Behavioral Axioms, Proactive Behaviors, Scent Anchor, Role Dynamic. Best on cards designed around this engine.<br><br>
▸ <strong><code>any_bots</code> — Universal edition.</strong> Self-contained. Works on cards not written around this engine. Carries its own structural rules without depending on Core-Card vocabulary or a paired lorebook.
</p>

Same spine. Different intake. Pick the one that matches how your card is written.

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

<p align="center"><sub>File naming: <code>{01–06}_{my_bots|any_bots}_{lite|full|multi}_v10_8_4_{lang}.txt</sub></code></p>

<p align="center">═════════════════════════</p>
<h2 align="center">『 🛠️ NOTES 』</h2>
<p align="center">═════════════════════════</p>

<p>
▸ <strong>Verification.</strong> Line counts ±0 across translations. HUD glyphs preserved: 🎯 💭 🧵 🔐 🎭 🌫 📚 ⏳ 🌐 📖. Operators preserved: ≥ ≤ ∈ ∧ ∨ → ±. Enum tokens translated via language-specific tables.<br><br>
▸ <strong>Optimized for.</strong> DeepSeek V4 Pro · DeepSeek V3.2 · DeepSeek R1 · Gemini 3.1 Pro · GLM 5.1 · Qwen 3.6 Max · Claude · GPT-4-class. Thinking mode strongly recommended for the flagship <code>full/</code> tier.<br><br>
▸ <strong>Platforms.</strong> Janitor.ai · SillyTavern · Chub.ai · Character Tavern · RisuAI. Anything that accepts a system / main / custom prompt.<br><br>
▸ <strong>Version.</strong> <code>v10.8.4</code> — hardened baseline. Numbering is build-internal; expect rare micro-patches to L0.5 anti-template lists, HUD slots, and enum tables. Pin a version in your character if you depend on exact behavior.
</p>

<p align="center">═════════════════════════</p>
<h2 align="center">💡 PRO TIP</h2>
<p align="center">═════════════════════════</p>

Watch the HUD. If `🧵 Thread` doesn't move for three posts, the engine is in stagnation territory — L2.6 should fire an outer disruption. If `🔐 Lock` isn't acknowledged in prose, the secret is leaking. If `🎯 Goal` reads as an abstract noun (*"connection"*, *"peace"*), the scene is template-drifting — rewrite it as an observable action.

<p align="center">═════════════════════════</p>
<h2 align="center">💬 FROM THE AUTHOR</h2>
<p align="center">═════════════════════════</p>

Ethereal Engine is the hardened form of a literary HUD prompt line developed since mid-2025. It exists because most "RP prompts" are either flowery permission slips or aesthetic flavor text — neither survives a long scene. This one is closer to a compiler than a vibe: it accepts a character card, enforces structural constraints, and refuses the easy bridge phrase.

If you build characters that need to remember, behave, refuse, escalate, hesitate, and *not collapse on turn fifteen* — this is the prompt I wish I'd had when I started.

<p align="center">═════════════════════════</p>

<p align="center">
  <em>Memory holds. The body answers first. The HUD keeps the truth.</em><br>
  <em>The room refuses to forget. Start the scene.</em>
</p>
