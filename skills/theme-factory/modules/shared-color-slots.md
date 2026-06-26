# Color Slots

## 14 Color Slots

| Slot            | Capture                                                         |
| --------------- | --------------------------------------------------------------- |
| `background`    | Dominant page/canvas color                                      |
| `surface`       | Card/panel (~3-5% lighter/darker than bg)                       |
| `surfaceAlt`    | Zebra rows, sidebar, modal (~8-10% shift from bg)               |
| `primary`       | Main brand/action - buttons, active nav, links                  |
| `primaryLight`  | Primary at ~25% opacity over white                              |
| `secondary`     | Supporting accent - pills, tags, secondary buttons              |
| `accent`        | Pop color - CTA highlights, progress bars                       |
| `text`          | Main body text                                                  |
| `textMuted`     | Captions, labels, placeholders                                  |
| `textOnPrimary` | Text ON primary (white or very dark based on primary luminance) |
| `border`        | Subtle separator / card outline                                 |
| `success`       | Status green                                                    |
| `warning`       | Status amber                                                    |
| `error`         | Status red                                                      |

Missing slots: derive from nearby slots using ratios above. Status colors: match saturation level of the found palette.
