# Path B: HTML Extraction

1. **Read** the file
2. **Multi-theme check** — look for multiple `:root` overrides, `[data-theme]`, `@media prefers-color-scheme`
3. **Mine colors in priority order:**

   | Priority | Source                                                        |
   | -------- | ------------------------------------------------------------- |
   | 1        | `:root { --color-* }` — use directly, resolve variable chains |
   | 2        | `body`, `header`, `.btn`, `.card` CSS rules                   |
   | 3        | Inline `style=""` on hero, navbar, CTA                        |
   | 4        | Tailwind/utility classes → map to hex                         |
   | 5        | External `<link>` — note existence, derive from inline clues  |

4. **Map** → 14 color slots; derive missing slots using ratios in `modules/shared-color-slots.md`
5. **Background** — check `body`, `html`, `.page`, `.wrapper` background properties
6. **Effects** — mine `box-shadow`, `backdrop-filter`, `background-clip`, gradients per selector
7. **Typography** — `font-family`/`font-size`/`font-weight`/`line-height` on `body`/`:root`; mono from `code`/`pre`
8. **Shape** — `border-radius` from `:root`, `.card`, `.btn`
9. **Design DNA** — derive: density from padding/gap sizes; elevation from box-shadow frequency; motionFeel from transition durations
10. **Context gap?** — if HTML is sparse, read `modules/shared-signal-table.md` and infer from class names, content tone, visual intent
11. **Name** — ask if not provided
12. **Anti-pattern gate** — read `modules/anti-patterns.md` and silently fix all violations
13. **Write** preset → **update** index
