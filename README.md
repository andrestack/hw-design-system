# Hinterland Web brand

Brand source for [hinterlandweb.com](https://hinterlandweb.com): the design system, LinkedIn carousels, brand assets and motion prototypes.

## What's here

| Folder | What |
| --- | --- |
| `design-system/` | The Hinterland Web design system: `README.md` (voice, colour, type, imagery, motion and carousel rules), `tokens.json` (colours for the dark and light themes, type styles, spacing, radii, shadows, carousel sizes) and component previews. Tokens are taken from the live site's CSS. |
| `assets/` | `logo.png` / `logo.webp` (128 × 128, the only size the site serves), `hero-sky.webp` (the painted sky, 2048 × 1152), `sky-mask.png` (soft mask of the moving sky area). |
| `carousels/telegram-bot/` | 8-slide LinkedIn carousel (1080 × 1350) about the Telegram voice-note bot, as editable `.dc.html` artboards, plus the post caption. |
| `prototypes/living-sky/` | WebGL "living sky" hero prototype: the painted sky drifts, the big swirl breathes, the cursor stirs it. No libraries. |

## Notes

- Images inside the carousel artboards point at the copies uploaded to the Claude design canvas (`/_blob/…` URLs). The originals live in `assets/`.
- Still to add: a high-resolution logo, and André's photo for the carousel's last slide (placeholder marked `[YOUR PHOTO]`).
- Carousels go to LinkedIn as a PDF document post: export all slides as one PDF.
