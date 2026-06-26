# Path C: Text Extraction

**Design quality mandate:** Create distinctive, production-grade themes. Avoid generic aesthetics — every decision must feel intentional and opinionated.

---

## Intent Resolution

**With context** → derive tone, style, typography, color, background, and layout from the provided description.

**Without context** → freely invent a distinctive theme. Choose the pairing with the most creative tension:

- **Tone:** Dark / Light / Colorful / Colorless
- **Style:** formal / Super-Unrealistic / brutally minimal / maximalist / retro-futuristic / editorial / brutalist / art deco / soft/pastel / industrial / Psychedelic Surreal

---

## Reference Tables

Read each file as needed during extraction:

| What you need             | Read                                    |
| ------------------------- | --------------------------------------- |
| Map user signals → tokens | `modules/shared-signal-table.md`        |
| Color palette rules       | `modules/shared-color-palette-rules.md` |
| Font pairings             | `modules/shared-typography.md`          |
| Border radius by style    | `modules/shared-shape.md`               |
| Background pattern choice | `modules/shared-background.md`          |
| Effects by mood/keyword   | `modules/shared-effects.md`             |

---

## Output

- Use `modules/preset-template.html` as structural base, but **design freely** to express the theme's full potential
- Include a visible tag block showing `tone` and `style` (e.g. `Dark · Retro-futuristic`)
- Showcase content must fit the theme's world — brutalist gets harsh editorial blocks; psychedelic gets flowing surreal sections
- All decisions must feel cohesive — every component reinforces the same singular aesthetic
- Choose a name reflecting the specific aesthetic (e.g. `midnight-telegraph`, `chrome-pastoral`, `acid-ledger`)

**Before writing:** Run the Anti-Pattern Gate (read `modules/anti-patterns.md`). Silently fix all violations found.
