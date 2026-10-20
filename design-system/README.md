Hinterland Web is André Silva's one-person web design and AI studio on the Sunshine Coast. Everything it makes should feel hand-made in a world of generated sameness: painted, calm, specific.

## Voice

- Write as **I**, one person talking to one business owner. Never "we", never "our team".
- Short sentences. Plain words a tradie would use. One idea per line.
- Lead with the problem the owner already feels, then what changed. Real outcomes over features.
- Dry, a little cheeky, never hype: "Straight numbers. Mostly." "Four businesses. Zero templates."
- Name real things: Telegram, voice notes, the board, the weekly report. When an example uses customer names, say "Names in the examples are made up."
- No emoji. The only ornament glyph is ✦, in `marker`.
- Australian spelling: colour, organise, enquiry.

## Colour

- Default to the **dark** theme: `background` navy with `foreground` text. The light (sage) theme exists for documents and print.
- `accent` teal is the only action colour: primary buttons, links, the one italic serif word in a headline. Use it once per view.
- Text on a teal fill is `on-accent`, never cream.
- `marker` gold underlines one key phrase per headline (thickness 0.06em, offset 0.14em) and colours ✦. Never use it for body text.
- Surfaces step `frame` → `background` → `muted`. Story cards about automation use `card-secondary`.
- Separate surfaces with a 1px `border`, not shadows. `shadow-2xl` is only for website screenshots floating over a surface.
- Over the painted sky, always lay the navy gradient: `sky-overlay-top` → `sky-overlay-mid` at 55% → `sky-overlay-bottom`.

## Type

- Geist for everything (`sans`), Geist Mono (`mono`) for timestamps and technical tags. Both load from Google Fonts.
- Headlines: `display-xl` or `heading-1`, weight 500–600, tracking -0.025em, `text-wrap: balance`.
- Every headline may carry **one** word in `accent-italic` (serif italic, `accent`), as in "in the age of *AI*." Never two.
- Eyebrows are uppercase `eyebrow` / `eyebrow-sm` in `muted-foreground`.
- Body copy is `body-sm` or `body` in `muted-foreground` on cards, `foreground` elsewhere. Keep lines under 65 characters.

## Shape and space

- Buttons and chips are pills (`radius-full`). Cards are `radius-2xl`. The hero and big image panels are `radius-4xl`.
- Spacing runs on a 4px base: `space-3` inside cards, `space-8` between cards, `space-12` between blocks.
- Layouts are left-aligned. Centre only a single closing line.

## Imagery

- The brand image is the **painted sky**: a Van Gogh-style swirling teal and cream sky over a single rock peak. Use `Imagery/hinterland-sky.webp` full-bleed with the sky overlay, or crop to the swirl.
- The logo is the same world in a disc: swirl, low gold sun, the peak. Use `Logos/hinterland-logo.png` on any surface; it needs no backing.
- Website work is shown as real screenshots in rounded frames with `shadow-2xl`.
- Photos of André: warm, natural light, cut out or in a `radius-4xl` frame. Never stock photos of people.
- Never generic tech imagery: no circuit boards, robots, glowing brains, blue-purple gradients.

## Motion

- The sky can move: a slow flow-field drift masked off the mountain, and a cursor stir. Nothing else loops.
- Headline lines enter with a soft blur-up (from 8px blur, 20px down, 0 opacity). Content is readable without it.
- Always honour `prefers-reduced-motion`: show the still image.

## LinkedIn carousels

- Slides are `slide-width` × `slide-height` (1080 × 1350), exported together as one PDF.
- Keep everything but backgrounds inside `slide-margin`.
- Slide 1 is the hook: the painted sky, one `display-xl`-scale headline with one `accent-italic` word, logo and name at the bottom.
- Middle slides are dark `background`, one idea each: a big headline, at most 30 words of body, an optional visual.
- The last slide is the call to action on the sky again: one sentence, the free audit, the website, André's face.
- Every slide carries a small footer: logo, "Hinterland Web", and the slide number as `03 / 08` in `mono-tag`.

## Iconography

- The site uses no icon set. Use plain text labels and the ✦ glyph. If an icon is ever needed, use a thin 1.5px line style in `foreground`, and flag it.
