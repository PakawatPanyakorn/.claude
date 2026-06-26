# Effects

## Capture

Mine or infer concrete CSS values for each slot. Absent → `'none'` or `0`. Never omit.

| Effect          | Capture                                                                               |
| --------------- | ------------------------------------------------------------------------------------- |
| Hero gradient   | Full `linear-gradient(...)` for header/hero/navbar bg                                 |
| Button gradient | Full gradient for CTA buttons                                                         |
| Card gradient   | Subtle gradient for card bg, or `none`                                                |
| Gradient text   | Gradient for `background-clip: text` on headlines                                     |
| Accent gradient | Decorative bars/dividers, or `none`                                                   |
| Glow            | `glowColor` hex + `glowBlur` px + sm/md/lg `box-shadow` values                        |
| Glass           | `glassBlur: Npx` + `glassTint: rgba(...)` + `backdropFilter: blur(Npx) saturate(N%)` |
| Gradient border | CSS gradient for `border-image`                                                       |
| Inset shadow    | Full `inset ...` box-shadow                                                           |
| Noise opacity   | `0-1` (0 if absent)                                                                   |
| Text shadow     | Full `text-shadow` for headings                                                       |
| Colored shadow  | Full tinted `box-shadow` on primary elements                                          |

---

## Generate

| Implies                             | Generate                                                                               |
| ----------------------------------- | -------------------------------------------------------------------------------------- |
| neon / glow / cyber / electric      | Full glow system: sm/md/lg `box-shadow` values                                         |
| glass / frosted / blur              | `glassBlur: 12px`, `glassTint: rgba(...)`, `backdropFilter: blur(12px) saturate(180%)` |
| gradient / gradient buttons         | `--gradient-hero`, `--gradient-button`, `--gradient-card` values                       |
| neumorphic / soft shadow / embossed | Dual inset shadows                                                                     |
| gradient border / rainbow border    | `linear-gradient` for `border-image`                                                   |
| minimal / flat / clean / no shadow  | All effects `none`                                                                     |
| (nothing implies it)                | `'none'` or `0` — never invent                                                         |
