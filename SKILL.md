---
name: color-skill
version: 1.0
description: Bold two-tone HTML color system from the user's palette screenshots. Use when the user says 컬러 스킬, color-skill, this color pattern, 컬러 패턴, 팔레트 HTML, or asks to make an HTML page/site/report with vivid paired color blocks, large rounded panels, high-contrast typography, Instagram-style palette cards, or strong complementary color rhythm.
---

# 컬러 스킬

HTML 화면을 만들 때 강한 보색 대비와 큰 컬러 블록으로 첫인상을 잡는다. 검은 무대 위에 색 패널을 놓고, 각 패널은 배경색과 글자색을 1:1로 강하게 맞물리게 만든다.

## Core Pattern

- Start with a black or near-black page background: `#000000`, `#050505`, or `#07090b`.
- Use large rounded color panels as the main visual structure. Radius may be `22px` to `32px` because this is the defining pattern.
- Each panel uses exactly one background color and one foreground color from the paired palette.
- Make text oversized, heavy, and simple. Prefer Inter, Pretendard, or system sans; `font-weight: 800-900`.
- Keep labels and controls as thin outlined pills using the same foreground color.
- Avoid gradients, glass blur, shadows, decorative blobs, beige-only pages, and low-contrast pastel washes.
- When multiple sections exist, alternate paired colors so the page feels like a stack of bold color cards.
- Korean text must use `word-break: keep-all; line-break: strict; overflow-wrap: break-word;`.

## Palette Pairs

Use these as locked pairs. The foreground color is also used for pill borders, dividers, arrows, icon strokes, and small labels.

| Name | Background | Foreground | Best Use |
|---|---:|---:|---|
| Violet | `#321847` | `#f15153` | premium, night, dramatic intro |
| Imperial Red | `#f15153` | `#321847` | punchy hero, CTA band, launch notice |
| Butter | `#ffefb3` | `#013e37` | soft readable section, quote, calm explainer |
| Green | `#013e37` | `#ffefb3` | trust, depth, serious product block |
| Cream Vanilla | `#efe6dd` | `#9a0002` | editorial intro, warm report section |
| Cherry Cola | `#9a0002` | `#efe6dd` | warning, decisive message, strong claim |
| Aureolin | `#fbe311` | `#261606` | bright key insight, number, announcement |
| Bistre | `#261606` | `#fbe311` | dark contrast panel, footer, proof block |
| Lime Green | `#d3f00a` | `#f9100c` | radical signal, youth, attention grab |
| Vibrant Red | `#f9100c` | `#d3f00a` | emergency CTA, campaign energy |

## HTML Layout Rules

- Build the first viewport around one large color panel, not a marketing-style split hero.
- Use black gutters between panels. The black negative space is part of the design, not empty filler.
- Keep panels full-width or nearly full-width on mobile; on desktop use constrained max width with generous vertical height.
- Use 2-column or 3-column grids only when each tile still preserves the two-tone rule.
- Put the most important sentence in the biggest text. Do not explain the visual system inside the app.
- Buttons: use filled foreground-on-background for primary action, outlined pills for secondary action.
- Tables and metric cards: color the container with one palette color; use the paired foreground for all text and rules.

## CSS Starter

Use or adapt this token shape when making HTML:

```css
:root {
  --black: #000000;
  --violet: #321847;
  --imperial-red: #f15153;
  --butter: #ffefb3;
  --green: #013e37;
  --cream-vanilla: #efe6dd;
  --cherry-cola: #9a0002;
  --aureolin: #fbe311;
  --bistre: #261606;
  --lime-green: #d3f00a;
  --vibrant-red: #f9100c;
}

body {
  margin: 0;
  background: var(--black);
  color: white;
  font-family: Inter, Pretendard, system-ui, -apple-system, BlinkMacSystemFont, sans-serif;
}

.color-panel {
  min-height: clamp(360px, 58vh, 680px);
  border-radius: clamp(22px, 3vw, 32px);
  padding: clamp(28px, 7vw, 96px);
  display: grid;
  align-content: center;
  gap: 28px;
  word-break: keep-all;
  line-break: strict;
  overflow-wrap: break-word;
}

.color-panel h1,
.color-panel h2 {
  margin: 0;
  color: var(--fg);
  font-size: clamp(48px, 10vw, 132px);
  line-height: 0.92;
  letter-spacing: 0;
  font-weight: 900;
}

.color-pill {
  width: fit-content;
  border: 1.5px solid currentColor;
  border-radius: 999px;
  color: var(--fg);
  padding: 12px 24px;
  font-weight: 700;
}
```

Example panel:

```html
<section class="color-panel" style="background:#321847; --fg:#f15153;">
  <h1>Violet Strategy</h1>
  <div class="color-pill">Hex -> #321847</div>
</section>
```

## Quality Gate

- Check every panel for readable contrast at mobile width and desktop width.
- Ensure long Korean headings wrap cleanly and never overflow the panel.
- If the page becomes one-note, add a second pair from the palette rather than tinting the same color.
- For visual HTML work, run a local preview and inspect the rendered page before final reporting whenever practical.
