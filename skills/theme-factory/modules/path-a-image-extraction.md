# Path A: Image Extraction

1. **Read** the image (Read tool — Claude has vision)
2. **Multi-theme check** — if multiple themes visible, present numbered list and wait for selection
3. **Colors** — analyze visually for all 14 slots (see `modules/shared-color-slots.md`)
4. **Typography** — serif/sans/mono feel; weight; density; choose a real matching font stack (see `modules/shared-typography.md`)
5. **Shape** — map feel to px (see `modules/shared-shape.md`)
6. **Background** — inspect canvas carefully before assuming solid (see `modules/shared-background.md`)
7. **Effects** — analyze visually (see `modules/shared-effects.md`)
8. **Design DNA** — assess overall language (see `modules/shared-color-slots.md`)
9. **Context gap?** — if image lacks detail, read `modules/shared-signal-table.md` and infer from color temperature, subject matter, overall mood
10. **Name** — ask "What would you like to name it?" (skip if auto mode or provided inline)
11. **Anti-pattern gate** — read `modules/anti-patterns.md` and silently fix all violations
12. **Write** preset HTML → **update** `index.html` THEMES array
