# Background

**Default: never use solid colors.** Every background must have at least two stacked techniques (gradient + texture, noise + mesh, etc.) unless the theme is explicitly plain, formal, or minimalist. Solid or near-solid colors are the last resort, not the default. Prefer gradient meshes, noise textures, geometric patterns, or layered transparencies, and stack multiple techniques for richness.

---

## Texture / Material Surfaces

| Implies                             | Generate                                                                                 |
| ----------------------------------- | ---------------------------------------------------------------------------------------- |
| paper / notebook / lined            | lines-h; warm off-white `#fdf6e3` base; 24px spacing; opacity 0.12                      |
| graph paper / grid                  | grid; `#e0e0e0` on white; 20px pitch; double-weight every 100px                         |
| dot grid / bullet journal           | dot-grid; `#b0b0b0` dots; 22px pitch; 1.5px radius                                      |
| blueprint / technical               | blueprint; `#0a2a4a` bg + `rgba(100,200,255,0.25)` grid lines; 20px pitch               |
| noise / grain / textured            | SVG feTurbulence noise overlay; `patternOpacity: 0.04`; blend mode `overlay`            |
| linen / canvas / fabric             | repeating diagonal crosshatch; warm `#f5efe6`; 4px pitch; opacity 0.18                  |
| cork / wood / organic               | layered radial + noise; warm browns `#c8a97a → #8b6240`; grain angle 15°                |
| concrete / brutalist                | grayscale noise `#888` on `#d4d0cc`; coarse turbulence `baseFrequency: 0.65`            |
| chalkboard / blackboard             | dark `#2b3a2b` base + fine noise; faint chalk-dust grain; `opacity: 0.06`               |

---

## Gradient & Mesh

| Implies                             | Generate                                                                                 |
| ----------------------------------- | ---------------------------------------------------------------------------------------- |
| gradient / mesh background          | CSS mesh via multiple `radial-gradient` blobs; 4–6 color stops; soft blend              |
| aurora / northern lights            | `conic-gradient` + radial overlays; `#00c6ff → #7b2ff7 → #ff6ec7`; animated shimmer    |
| sunset / dusk / golden hour         | `linear-gradient(160deg, #ff6a00, #ee0979, #2d1b69)`; light flare at top-right          |
| ocean / deep sea                    | `linear-gradient(180deg, #0077b6, #023e8a, #03045e)`; caustic light ripples overlay     |
| forest / nature / earthy            | `linear-gradient(135deg, #2d6a4f, #1b4332, #081c15)` + leaf-silhouette noise            |
| fire / ember / lava                 | radial burst `#ff4500 → #8b0000 → #1a0000`; particle-dot overlay; animated flicker      |
| neon glow / cyberpunk               | `#0d0d0d` base; radial neon blobs `#ff00ff, #00ffff, #ff6600`; glow blur 80px           |
| pastel dream / soft                 | mesh of `#fbc2eb, #a6c1ee, #ffecd2, #cfd9df`; 40% opacity blobs; very low contrast     |
| monochrome gradient                 | two-tone same-hue gradient; `0%` sat → `100%` sat; angle 135°                           |

---

## Geometric & Structural

| Implies                              | Generate                                                                                 |
| ------------------------------------ | ---------------------------------------------------------------------------------------- |
| plain / formal / minimal (explicit)  | solid only when theme keyword is "plain", "formal", "corporate", or "minimal"; `image: none` — **avoid for all other themes** |
| hexagon / honeycomb                  | SVG hex tiling; stroke `rgba(255,255,255,0.1)`; fill transparent; 48px cell             |
| triangles / low-poly                 | SVG Delaunay-style triangle mesh; flat shading; subtle hue variation per face            |
| chevron / herringbone                | repeating chevron SVG; 20px pitch; soft contrast `opacity: 0.12`                        |
| circuit board / PCB                  | dark `#0a1628` bg; mint trace lines `#00ff9d`; via dots; trace opacity 0.18             |
| isometric / 3D grid                  | isometric cube grid SVG; `rgba(255,255,255,0.07)` strokes on dark bg                    |
| topographic / contour map            | SVG concentric irregular curves; same-hue strokes; 8px step spacing; opacity 0.2        |
| Voronoi / organic cells              | SVG Voronoi diagram; thin cell borders; fills from analogous palette; low opacity        |
| diagonal stripes / awning            | `repeating-linear-gradient(45deg, color1 0 10px, color2 10px 20px)`                      |
| crosshatch / etching                 | two-layer diagonal lines 45° + 135°; thin stroke; opacity 0.08; warm tones              |

---

## Atmospheric & Cosmic

| Implies                              | Generate                                                                                 |
| ------------------------------------ | ---------------------------------------------------------------------------------------- |
| stars / night sky / space            | `#000510` base; scattered white dots 0.5–2px; radial glow center; nebula blobs optional |
| milky way / galaxy                   | dark base + radial gradient band `rgba(180,160,255,0.15)`; star-field noise overlay     |
| clouds / dreamy / soft sky           | `#87ceeb` base; layered white radial gradients; blur 60–120px; wispy motion             |
| fog / mist / atmospheric             | `linear-gradient` light grey base; overlapping white radial spots; blur 100px           |
| rain / storm / moody                 | dark `#1a1f2e` base; vertical noise streaks `opacity: 0.05`; blue-grey ambient          |
| snow / winter / frost                | white/ice `#e8f4fc` base; scattered dot snowflakes; cold blue vignette                  |
| smoke / vapor / ethereal             | `#111` base; slow-moving white Gaussian blobs; `mix-blend-mode: screen`                 |

---

## Brand & Art Direction

| Implies                              | Generate                                                                                 |
| ------------------------------------ | ---------------------------------------------------------------------------------------- |
| retro / vaporwave / 80s              | `#2d1b69` base; grid floor `perspective(300px)`; scanlines `opacity: 0.04`; pink+cyan   |
| vintage / sepia / aged               | warm `#f0e6d0` base; brown noise grain; vignette edges; muted saturation                |
| glassmorphism / frosted              | semi-transparent `rgba(255,255,255,0.08)` + backdrop blur 20px over vivid blurred bg   |
| neumorphism / soft-UI                | flat grey `#e0e5ec`; inset shadow `#babecc` + `#ffffff`; zero texture                   |
| brutalism / raw                      | solid block color; hard-edge stripe overlay; zero border-radius; high contrast          |
| Japanese / washi / zen               | off-white `#f8f4ee` base; very faint sumi-ink brush stroke SVGs; cloud border motif     |
| art deco / gatsby                    | deep `#1a1200` base; gold `#d4af37` geometric fan rays; 2px borders; symmetry           |
| Memphis / 80s graphic design         | white base; scattered small geometric shapes (triangles, squiggles, dots); bold palette |
| watercolor / painterly               | soft bleed blobs; wet-edge opacity falloff; analogous palette; no hard lines            |

---

## Stacking Guide

Combine layers in this order for richness without muddle:

```
1. Base color / solid or coarse gradient  ← lowest
2. Primary texture (grid, dots, noise)
3. Gradient overlay (mesh, atmospheric bloom)
4. Vignette / edge darkening              ← highest
```

Opacity budget per layer: base 100% → texture ≤ 15% → overlay ≤ 30% → vignette ≤ 40%.

**Minimum requirement:** every non-plain/non-formal theme must use at least layers 1 + 2 (base + texture or gradient). A single solid color with no texture or gradient is a failure condition.
