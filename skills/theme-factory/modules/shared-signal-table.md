# Signal Table

| Signal     | Examples                                                                                                          | Maps to                                                       |
| ---------- | ----------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------- |
| Tone       | dark, light, colorful, colorless                                                                                  | Overall lightness/saturation → color slot values              |
| Style      | brutalist, art deco, editorial, surreal, formal, maximalist, retro-futuristic, soft/pastel, industrial, psychedelic | Aesthetic direction → `shared-color-palette-rules.md`        |
| Hue        | blue, teal, warm orange, purple                                                                                   | `primary`, `accent`, `secondary` slots                        |
| Background | dark terminal, white paper, off-white, dot grid, blueprint, noise/paper                                           | `background` slot + pattern type → `shared-background.md`    |
| Typography | serif editorial, monospace code, geometric sans, high contrast                                                    | Font stacks + weight/size scale → `shared-typography.md`      |
| Shape      | sharp, rounded, pill, angular                                                                                     | `borderRadius` values → `shared-shape.md`                     |
| Effects    | glow, glass, gradient text, noise, inset shadow, gradient border                                                  | Effect tokens (glow/glass/gradients) → `shared-effects.md`   |
| Reference  | "like GitHub dark", "like Notion", "like Linear"                                                                  | Match known palette closely across all 14 slots               |
| Mood       | cyberpunk, minimal, corporate, warm, editorial, brutally minimal                                                  | Saturation, contrast, spacing, elevation density              |
