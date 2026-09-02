# Altitude — Style Reference
> midnight financial editorial — a darkened trading floor printed on bone-white serif stock, lit only by thin borders and a single blue accent.

**Theme:** dark

Altitude operates in a midnight editorial register: near-black canvas, off-white serif headlines (Libre Baskerville), and razor-thin secondary type (Inter). The serif-on-dark pairing is the signature — most AI finance tools lean on geometric sans-serifs; Altitude borrows from financial print (WSJ, FT) to signal authority and discretion. Mountain ridge linework and painterly landscape photography replace the usual gradient meshes and 3D renders, grounding the AI product in a sense of summit and scale. Surfaces are stratified by barely-perceptible gray steps (#111 → #181 → #1f → #26 → #32), with hairline borders doing the structural work that shadows do elsewhere. Color is almost entirely absent from the interface — when it appears, it reads as functional punctuation rather than decoration. Components are tight, rectangular (4–8px radii), and content-forward.

## Tokens — Colors

| Name | Value | Token | Role |
|------|-------|-------|------|
| Carbon Canvas | `#181818` | `--color-carbon-canvas` | Primary page background; the foundational dark surface that all sections sit on |
| Obsidian | `#111111` | `--color-obsidian` | Deepest layer — footer, contrast blocks, shadow wells |
| Graphite Card | `#1f1f1f` | `--color-graphite-card` | Card and input surfaces lifted one step above canvas |
| Slate Elevated | `#262626` | `--color-slate-elevated` | Elevated surfaces — table rows, hover states, secondary panels |
| Iron Peak | `#323232` | `--color-iron-peak` | Highest surface tier — dropdowns, popovers, selected list items |
| Bone | `#eeeeee` | `--color-bone` | Primary text and hairline borders — the dominant foreground tone |
| Ash | `#e4e4e4` | `--color-ash` | Secondary borders and card outlines |
| Fog | `#a4a19b` | `--color-fog` | Muted helper text, icon strokes, disabled labels |
| Smoke | `#5e5d59` | `--color-smoke` | Subtle dividers, badge backgrounds, low-emphasis text |
| Pewter | `#4b4b4b` | `--color-pewter` | Deep borders, table separators |
| Pure White | `#ffffff` | `--color-pure-white` | Icon glyphs, card backgrounds for light-section contrast blocks, max-emphasis text |
| Voltage Blue | `#2b7fff` | `--color-voltage-blue` | Sole chromatic accent — inline link highlights, selection, active state within data-dense terminal views; appears as the only color in an otherwise achromatic system |
| Mid Navy | `#1a365d` | `--color-mid-navy` | Decorative deep-blue tone used in heading borders and subtle heading tints — adds depth without breaking the monochromatic discipline |

## Tokens — Typography

### Libre Baskerville — Display headlines exclusively (hero, section openers). The serif choice on a dark canvas is the brand's most distinctive move — it borrows financial-print authority (FT, Barron's) and makes an AI product feel like a private journal rather than a dashboard. Always weight 400 or 500; never bold. Letter-spacing tightens at -0.025em to keep long phrases compact. · `--font-libre-baskerville`
- **Substitute:** Source Serif Pro, Lora, Crimson Text
- **Weights:** 400, 500
- **Sizes:** 36px, 48px, 72px
- **Line height:** 1.10, 1.15, 1.25
- **Letter spacing:** -0.0250em
- **Role:** Display headlines exclusively (hero, section openers). The serif choice on a dark canvas is the brand's most distinctive move — it borrows financial-print authority (FT, Barron's) and makes an AI product feel like a private journal rather than a dashboard. Always weight 400 or 500; never bold. Letter-spacing tightens at -0.025em to keep long phrases compact.

### Inter — All functional UI — body, nav, buttons, inputs, table cells, badges, captions. Weight 400 is the default; 500–600 for emphasis. The 8–11px range is used aggressively for data-dense terminal/table contexts, and the positive letter-spacing (0.025–0.05em) applies to small uppercase labels and badges to compensate for size. · `--font-inter`
- **Substitute:** system-ui, -apple-system, Segoe UI
- **Weights:** 400, 500, 600, 700
- **Sizes:** 8px, 9px, 10px, 11px, 12px, 13px, 14px, 16px, 18px, 28px
- **Line height:** 1.20, 1.25, 1.33, 1.38, 1.43, 1.50, 1.63
- **Letter spacing:** -0.0250em, 0.0250em, 0.0500em
- **Role:** All functional UI — body, nav, buttons, inputs, table cells, badges, captions. Weight 400 is the default; 500–600 for emphasis. The 8–11px range is used aggressively for data-dense terminal/table contexts, and the positive letter-spacing (0.025–0.05em) applies to small uppercase labels and badges to compensate for size.

### Fira Code — Monospaced contexts — code blocks, query inputs, and data identifiers within the terminal-style product UI. The +0.1em tracking is signature for code labels and command strings. · `--font-fira-code`
- **Substitute:** JetBrains Mono, IBM Plex Mono
- **Weights:** 400, 600
- **Sizes:** 10px, 14px, 16px
- **Line height:** 1.43, 1.50
- **Letter spacing:** 0.1000em
- **Role:** Monospaced contexts — code blocks, query inputs, and data identifiers within the terminal-style product UI. The +0.1em tracking is signature for code labels and command strings.

### Type Scale

| Role | Size | Line Height | Letter Spacing | Token |
|------|------|-------------|----------------|-------|
| caption | 10px | 1.5 | 0.5px | `--text-caption` |
| body | 14px | 1.5 | — | `--text-body` |
| heading-sm | 18px | 1.43 | -0.45px | `--text-heading-sm` |
| heading | 28px | 1.38 | -0.7px | `--text-heading` |
| heading-lg | 36px | 1.15 | -0.9px | `--text-heading-lg` |
| display | 72px | 1.1 | -1.8px | `--text-display` |

## Tokens — Spacing & Shapes

**Base unit:** 4px

**Density:** comfortable

### Spacing Scale

| Name | Value | Token |
|------|-------|-------|
| 4 | 4px | `--spacing-4` |
| 8 | 8px | `--spacing-8` |
| 12 | 12px | `--spacing-12` |
| 16 | 16px | `--spacing-16` |
| 20 | 20px | `--spacing-20` |
| 24 | 24px | `--spacing-24` |
| 32 | 32px | `--spacing-32` |
| 48 | 48px | `--spacing-48` |
| 64 | 64px | `--spacing-64` |
| 80 | 80px | `--spacing-80` |
| 96 | 96px | `--spacing-96` |
| 128 | 128px | `--spacing-128` |
| 136 | 136px | `--spacing-136` |
| 224 | 224px | `--spacing-224` |

### Border Radius

| Element | Value |
|---------|-------|
| cards | 8px |
| icons | 4px |
| badges | 4px |
| inputs | 4px |
| buttons | 4px |
| large_surfaces | 16px |

### Shadows

| Name | Value | Token |
|------|-------|-------|
| md | `rgba(51, 51, 51, 0.05) 0px 2px 15px 0px, rgba(51, 51, 51,...` | `--shadow-md` |
| subtle | `oklab(0 0 0 / 0.2) 0px 0px 0px 1px, rgba(51, 51, 51, 0.05...` | `--shadow-subtle` |
| subtle-2 | `oklab(0.999994 0.0000455678 0.0000200868 / 0.1) 0px 0px 0...` | `--shadow-subtle-2` |
| subtle-3 | `oklab(0.95 0 0 / 0.1) 0px 0px 0px 1px` | `--shadow-subtle-3` |
| subtle-4 | `rgb(232, 110, 88) 0px 0px 0px 2px, rgba(51, 51, 51, 0.05)...` | `--shadow-subtle-4` |

### Layout

- **Page max-width:** 1200px
- **Section gap:** 80px
- **Card padding:** 12px
- **Element gap:** 8px

## Components

### Ghost Button
**Role:** Primary CTA — used for 'Request a Demo' and navigation actions

Transparent background, 1px solid #eeeeee border, #eeeeee text at 14px Inter weight 500, 4px radius, 16px horizontal / 8px vertical padding. Hover lifts to #262626 background. The filled-inverse version (white bg, black text) is rare; the ghost is the default voice.

### Navigation Link
**Role:** Top nav items (Platform, Security, Blog)

No background, no border. Inter 14px weight 400 in #eeeeee. Active state: 1px #aeaeae bottom border acting as a thin underline marker. Sits in a 64px-tall bar with the wordmark left and Login right.

### Workflow Tile
**Role:** Feature card within the automated workflows grid

Off-white card (#e7e5e4 to #ffffff range) on the dark canvas, 8px radius, 24px padding. Centered icon (24px, 1.5px stroke) in #1a365d, label beneath in Inter 13px weight 500, #181818 text. Arranged in a 5-column grid with 12px gaps.

### Terminal Window
**Role:** Product screenshot / app frame overlay

Dark app chrome (#1f1f1f) with traffic-light dots (red/yellow/green) top-left, sidebar listing platform items in Inter 13px, and a main content area with Fira Code monospaced text. Rounded 8px on the container; the internal panes are square-cornered. Drops the heavy modal-level shadow when presented as a marketing screenshot.

### Serif Section Header
**Role:** Section openers (e.g. 'Sherpa — Your AI Analyst', 'Automated Workflows')

Libre Baskerville 48px weight 400, #eeeeee, line-height 1.15, letter-spacing -0.025em. No kicker label, no eyebrow — the serif does all the work. Subhead below in Inter 16px weight 400, #a4a19b.

### Hero Composition
**Role:** Above-the-fold hero block

Full-viewport #181818 canvas. Centered stack: display headline (Libre Baskerville 72px, #eeeeee, ls -0.025em), single-line subhead (Inter 18px, #a4a19b), ghost CTA below. A continuous mountain ridge line in 1px #a4a19b runs full-width near the bottom — the only decorative graphic on the page.

### Input Field
**Role:** Form inputs, search bars, query fields

Background #1f1f1f, 1px #323232 border, 4px radius, 12px padding, Inter 14px weight 400, #eeeeee text. Placeholder in #5e5d59. Focus ring: 2px #2b7fff outer glow.

### Badge / Status Pill
**Role:** Tags, status indicators, category labels

Background #5e5d59 or #323232, text Inter 11px weight 500 in #eeeeee, 4px radius, 6px 10px padding. Uppercase tracking +0.05em. No colored fill — status is always communicated through border weight or text, never hue.

### Data Table Row
**Role:** Row within terminal-style data tables

Background alternates between transparent and #262626; 1px #262626 bottom border; Inter 13px weight 400 in #eeeeee; 16px vertical padding. Header row uses Inter 11px weight 500 uppercase, tracking +0.05em, in #a4a19b.

### Product Feature Split
**Role:** Two-column section: copy left, product visual right

Max-width 1200px centered. Left column: 40% width, serif heading + body copy + text-link CTA ('Try Me →'). Right column: 60% width, product visual (terminal window over mountain landscape) with 8px container radius. Section gap 80px above and below.

### Footer
**Role:** Page footer

Background #111111, 64px vertical padding. Wordmark, nav links, and legal in Inter 13px weight 400, #a4a19b. 1px #1f1f1f top border separates from main content.

### Image Card / Hero Visual
**Role:** Photographic or illustrated visuals with rounded container

16px radius, 1px #262626 border, #1f1f1f fallback background behind image. Mountain landscape photography (painterly, blue-gray, atmospheric) is the primary visual — no abstract gradients, no 3D renders.

## Do's and Don'ts

### Do
- Use Libre Baskerville weight 400 at 36–72px for all section and display headlines; never substitute a sans-serif for these.
- Maintain the surface stack: #111 → #181 → #1f → #26 → #32, ascending by roughly 5–10% luminance steps.
- Use 4px radius for all buttons, inputs, and badges; 8px for cards; 16px only for large image containers.
- Keep body text in Inter 14px weight 400, #eeeeee, with #a4a19b for muted helper text and #5e5d59 for placeholders.
- Use 8px element gaps and 12px card padding as the baseline; scale section rhythm in 24/32/64/80px steps.
- Let the mountain ridge line graphic or landscape photography do the visual storytelling — no gradient meshes, no 3D orbs, no neon glows.
- Communicate status through weight, border, and tracking rather than color; reserve #2b7fff for inline links and the focus ring only.

### Don't
- Don't use bold weights (700) for headlines — Libre Baskerville at weight 400 is the voice; going heavier breaks the editorial register.
- Don't introduce new accent colors — the system is monochromatic with one blue; adding green/red/yellow for semantic states breaks the discipline.
- Don't use heavy drop shadows for cards or buttons; shadows here are 0.05 opacity whispers, not 0.3-opacity lifts.
- Don't round corners above 16px — the rectilinear 4–8px language is a signature; pill shapes (9999px) would look foreign.
- Don't use white (#ffffff) as body text — #eeeeee is softer and the right foreground tone against #181818.
- Don't pair Inter with another sans-serif for headings; the Inter/Baskerville duality is the only pairing the system uses.
- Don't apply gradients to UI surfaces — the one detected gradient is on a landscape image, not on any card or button.

## Surfaces

| Level | Name | Value | Purpose |
|-------|------|-------|---------|
| 0 | Obsidian | `#111111` | Deepest base — footer wells, contrast blocks beneath cards |
| 1 | Carbon Canvas | `#181818` | Primary page background |
| 2 | Graphite Card | `#1f1f1f` | Cards, inputs, contained surfaces |
| 3 | Slate Elevated | `#262626` | Hover states, table rows, secondary panels |
| 4 | Iron Peak | `#323232` | Top elevation — popovers, dropdowns, active selections |

## Elevation

- **Card:** `0px 2px 15px 0px rgba(51,51,51,0.05), 0px 1px 2px -1px rgba(51,51,51,0.05)`
- **Button:** `0px 0px 0px 1px oklab(0 0 0 / 0.2), 0px 2px 15px 0px rgba(51,51,51,0.05), 0px 1px 2px -1px rgba(51,51,51,0.05)`
- **Modal / Overlay:** `0px 0px 0px 1px oklab(0.999994 0.0000455678 0.0000200868 / 0.1), 0px 8px 24px 0px rgba(0,0,0,0.3), 0px 2px 8px 0px rgba(0,0,0,0.2)`

## Imagery

Photography is the dominant visual medium — specifically painterly, atmospheric mountain landscapes in muted blue-grays that evoke summit, scale, and distance. These appear as full-bleed or large contained images behind product terminal screenshots, creating a 'looking through a window at the product' effect. A continuous single-line mountain ridge SVG runs across the hero, drawn in 1px #a4a19b — a minimalist line-art counterpoint to the photographic sections. Icons are outline-style, 1.5px stroke, monochrome in #1a365d or #a4a19b, never filled. No 3D renders, no abstract gradient art, no stock-style lifestyle photography. The imagery vocabulary is: landscape photography + thin line-art + product terminal screenshots.

## Layout

Max-width 1200px centered, full-bleed dark canvas. Hero is a centered single-column stack (display headline → subhead → ghost CTA) with the mountain ridge line running full-width at the bottom. Product sections alternate between two patterns: (1) a dark product-visual-right layout (40% copy left, 60% terminal-over-landscape right) and (2) a dark copy-right layout with a light off-white workflow card grid on the left. Section gaps are generous — 80px vertical rhythm separates each band. Navigation is a single 64px-tall top bar with the wordmark left, three nav links center, Login right; no sticky behavior, no hamburger. The page flows seamlessly from dark to dark with one light-section interruption (the workflow grid) for contrast.

## Agent Prompt Guide

**Quick Color Reference**
- text: #eeeeee
- background: #181818
- border: #262626
- accent: #2b7fff
- muted text: #a4a19b
- primary action: no distinct CTA color

**3-5 Example Component Prompts**

No distinct primary action color was observed; use the extracted neutral button treatments instead of inventing a filled CTA color.

2. **Serif section header + body**: Left-aligned Libre Baskerville 48px weight 400, #eeeeee, letter-spacing -1.2px. Subhead in Inter 16px weight 400, #a4a19b. Body copy in Inter 14px weight 400, #eeeeee, 1.5 line-height. 'Try Me →' text link in Inter 14px weight 500, #2b7fff.

3. **Workflow tile card**: Off-white #e7e5e4 background, 8px radius, 24px padding, 1px #e4e4e4 border. Centered 24px outline icon in #1a365d. Label beneath in Inter 13px weight 500, #181818. Arranged in a 5-column grid with 12px gaps on the #181818 canvas.

4. **Terminal window**: #1f1f1f background, 8px radius, 1px #262626 border. Top bar with three 10px traffic-light dots (red #ff5f57, yellow #febc20, green #28c840). Sidebar at 200px width with Inter 13px #eeeeee list items on #181818 background. Main pane with Fira Code 14px, #eeeeee text on #1f1f1f.

5. **Data table row**: Full-width row, 16px vertical padding, 1px #262626 bottom border. Inter 13px weight 400, #eeeeee. Alternating row background: transparent and #262626. Header row above: Inter 11px weight 500 uppercase, +0.5px tracking, #a4a19b.

## Similar Brands

- **Ramp** — Same near-black canvas with generous serif/sans pairing, monochromatic discipline, and ghost-button CTAs — though Ramp is lighter and more playful.
- **Plaid** — Dark-mode fintech surface with thin borders, hairline structural elements, and restrained color use; similar density and information-forward layout.
- **Linear** — Dark dense UI with the same five-step gray surface stack, 4–8px corner radius vocabulary, and the same 'chromatic accent only where functionally necessary' rule.
- **Bloomberg Terminal** — Shares the editorial-financial DNA — serif display, monospaced data, dark canvas, hairline grid lines, and zero tolerance for decorative color.

## Quick Start

### CSS Custom Properties

```css
:root {
  /* Colors */
  --color-carbon-canvas: #181818;
  --color-obsidian: #111111;
  --color-graphite-card: #1f1f1f;
  --color-slate-elevated: #262626;
  --color-iron-peak: #323232;
  --color-bone: #eeeeee;
  --color-ash: #e4e4e4;
  --color-fog: #a4a19b;
  --color-smoke: #5e5d59;
  --color-pewter: #4b4b4b;
  --color-pure-white: #ffffff;
  --color-voltage-blue: #2b7fff;
  --color-mid-navy: #1a365d;

  /* Typography — Font Families */
  --font-libre-baskerville: 'Libre Baskerville', ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
  --font-inter: 'Inter', ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
  --font-fira-code: 'Fira Code', ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, monospace;

  /* Typography — Scale */
  --text-caption: 10px;
  --leading-caption: 1.5;
  --tracking-caption: 0.5px;
  --text-body: 14px;
  --leading-body: 1.5;
  --text-heading-sm: 18px;
  --leading-heading-sm: 1.43;
  --tracking-heading-sm: -0.45px;
  --text-heading: 28px;
  --leading-heading: 1.38;
  --tracking-heading: -0.7px;
  --text-heading-lg: 36px;
  --leading-heading-lg: 1.15;
  --tracking-heading-lg: -0.9px;
  --text-display: 72px;
  --leading-display: 1.1;
  --tracking-display: -1.8px;

  /* Typography — Weights */
  --font-weight-regular: 400;
  --font-weight-medium: 500;
  --font-weight-semibold: 600;
  --font-weight-bold: 700;

  /* Spacing */
  --spacing-unit: 4px;
  --spacing-4: 4px;
  --spacing-8: 8px;
  --spacing-12: 12px;
  --spacing-16: 16px;
  --spacing-20: 20px;
  --spacing-24: 24px;
  --spacing-32: 32px;
  --spacing-48: 48px;
  --spacing-64: 64px;
  --spacing-80: 80px;
  --spacing-96: 96px;
  --spacing-128: 128px;
  --spacing-136: 136px;
  --spacing-224: 224px;

  /* Layout */
  --page-max-width: 1200px;
  --section-gap: 80px;
  --card-padding: 12px;
  --element-gap: 8px;

  /* Border Radius */
  --radius-md: 4px;
  --radius-lg: 8px;
  --radius-2xl: 16px;

  /* Named Radii */
  --radius-cards: 8px;
  --radius-icons: 4px;
  --radius-badges: 4px;
  --radius-inputs: 4px;
  --radius-buttons: 4px;
  --radius-largesurfaces: 16px;

  /* Shadows */
  --shadow-md: rgba(51, 51, 51, 0.05) 0px 2px 15px 0px, rgba(51, 51, 51, 0.05) 0px 1px 2px -1px;
  --shadow-subtle: oklab(0 0 0 / 0.2) 0px 0px 0px 1px, rgba(51, 51, 51, 0.05) 0px 2px 15px 0px, rgba(51, 51, 51, 0.05) 0px 1px 2px -1px;
  --shadow-subtle-2: oklab(0.999994 0.0000455678 0.0000200868 / 0.1) 0px 0px 0px 1px, rgba(0, 0, 0, 0.3) 0px 8px 24px 0px, rgba(0, 0, 0, 0.2) 0px 2px 8px 0px;
  --shadow-subtle-3: oklab(0.95 0 0 / 0.1) 0px 0px 0px 1px;
  --shadow-subtle-4: rgb(232, 110, 88) 0px 0px 0px 2px, rgba(51, 51, 51, 0.05) 0px 2px 15px 0px, rgba(51, 51, 51, 0.05) 0px 1px 2px -1px;

  /* Surfaces */
  --surface-obsidian: #111111;
  --surface-carbon-canvas: #181818;
  --surface-graphite-card: #1f1f1f;
  --surface-slate-elevated: #262626;
  --surface-iron-peak: #323232;
}
```

### Tailwind v4

```css
@theme {
  /* Colors */
  --color-carbon-canvas: #181818;
  --color-obsidian: #111111;
  --color-graphite-card: #1f1f1f;
  --color-slate-elevated: #262626;
  --color-iron-peak: #323232;
  --color-bone: #eeeeee;
  --color-ash: #e4e4e4;
  --color-fog: #a4a19b;
  --color-smoke: #5e5d59;
  --color-pewter: #4b4b4b;
  --color-pure-white: #ffffff;
  --color-voltage-blue: #2b7fff;
  --color-mid-navy: #1a365d;

  /* Typography */
  --font-libre-baskerville: 'Libre Baskerville', ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
  --font-inter: 'Inter', ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
  --font-fira-code: 'Fira Code', ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, monospace;

  /* Typography — Scale */
  --text-caption: 10px;
  --leading-caption: 1.5;
  --tracking-caption: 0.5px;
  --text-body: 14px;
  --leading-body: 1.5;
  --text-heading-sm: 18px;
  --leading-heading-sm: 1.43;
  --tracking-heading-sm: -0.45px;
  --text-heading: 28px;
  --leading-heading: 1.38;
  --tracking-heading: -0.7px;
  --text-heading-lg: 36px;
  --leading-heading-lg: 1.15;
  --tracking-heading-lg: -0.9px;
  --text-display: 72px;
  --leading-display: 1.1;
  --tracking-display: -1.8px;

  /* Spacing */
  --spacing-4: 4px;
  --spacing-8: 8px;
  --spacing-12: 12px;
  --spacing-16: 16px;
  --spacing-20: 20px;
  --spacing-24: 24px;
  --spacing-32: 32px;
  --spacing-48: 48px;
  --spacing-64: 64px;
  --spacing-80: 80px;
  --spacing-96: 96px;
  --spacing-128: 128px;
  --spacing-136: 136px;
  --spacing-224: 224px;

  /* Border Radius */
  --radius-md: 4px;
  --radius-lg: 8px;
  --radius-2xl: 16px;

  /* Shadows */
  --shadow-md: rgba(51, 51, 51, 0.05) 0px 2px 15px 0px, rgba(51, 51, 51, 0.05) 0px 1px 2px -1px;
  --shadow-subtle: oklab(0 0 0 / 0.2) 0px 0px 0px 1px, rgba(51, 51, 51, 0.05) 0px 2px 15px 0px, rgba(51, 51, 51, 0.05) 0px 1px 2px -1px;
  --shadow-subtle-2: oklab(0.999994 0.0000455678 0.0000200868 / 0.1) 0px 0px 0px 1px, rgba(0, 0, 0, 0.3) 0px 8px 24px 0px, rgba(0, 0, 0, 0.2) 0px 2px 8px 0px;
  --shadow-subtle-3: oklab(0.95 0 0 / 0.1) 0px 0px 0px 1px;
  --shadow-subtle-4: rgb(232, 110, 88) 0px 0px 0px 2px, rgba(51, 51, 51, 0.05) 0px 2px 15px 0px, rgba(51, 51, 51, 0.05) 0px 1px 2px -1px;
}
```
</code></pre></div></div></div></div></div></main></div><script>$RS=function(a,b){a=document.getElementById(a);b=document.getElementById(b);for(a.parentNode.removeChild(a);a.firstChild;)b.parentNode.insertBefore(a.firstChild,b);b.parentNode.removeChild(b)};$RS("S:2","P:2")</script><div hidden id="S:4"><span>Don't use heavy drop shadows for cards or buttons; shadows here are 0.05 opacity whispers, not 0.3-opacity lifts.</span></div><script>$RS("S:4","P:4")</script><div hidden id="S:5"><li class="flex items-start gap-2 text-sm text-foreground"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-x mt-0.5 size-4 shrink-0 text-red-500" aria-hidden="true"><path d="M18 6 6 18"></path><path d="m6 6 12 12"></path></svg><span>Don't round corners above 16px — the rectilinear 4–8px language is a signature; pill shapes (9999px) would look foreign.</span></li></div><script>$RS("S:5","P:5")</script><div hidden id="S:6"><li class="flex items-start gap-2 text-sm text-foreground"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-x mt-0.5 size-4 shrink-0 text-red-500" aria-hidden="true"><path d="M18 6 6 18"></path><path d="m6 6 12 12"></path></svg><span>Don't use white (#ffffff) as body text — #eeeeee is softer and the right foreground tone against #181818.</span></li></div><script>$RS("S:6","P:6")</script><div hidden id="S:7"><li class="flex items-start gap-2 text-sm text-foreground"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-x mt-0.5 size-4 shrink-0 text-red-500" aria-hidden="true"><path d="M18 6 6 18"></path><path d="m6 6 12 12"></path></svg><span>Don't pair Inter with another sans-serif for headings; the Inter/Baskerville duality is the only pairing the system uses.</span></li></div><script>$RS("S:7","P:7")</script><div hidden id="S:8"><li class="flex items-start gap-2 text-sm text-foreground"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-x mt-0.5 size-4 shrink-0 text-red-500" aria-hidden="true"><path d="M18 6 6 18"></path><path d="m6 6 12 12"></path></svg><span>Don't apply gradients to UI surfaces — the one detected gradient is on a landscape image, not on any card or button.</span></li></div><script>$RS("S:8","P:8")</script><script>$RC("B:1","S:1")</script><script>self.__next_f.push([1,"3b:I[55925,[\"/_next/static/chunks/0mrygax_2m132.js?dpl=dpl_BdwYag37Coka3wCmVQYgfikUc21G\",\"/_next/static/chunks/0d3shmwh5_nmn.js?dpl=dpl_BdwYag37Coka3wCmVQYgfikUc21G\",\"/_next/static/chunks/0w9zxh-w3z4bi.js?dpl=dpl_BdwYag37Coka3wCmVQYgfikUc21G\",\"/_next/static/chunks/023b0pevwkepq.js?dpl=dpl_BdwYag37Coka3wCmVQYgfikUc21G\",\"/_next/static/chunks/11ktc8fnxphx8.js?dpl=dpl_BdwYag37Coka3wCmVQYgfikUc21G\",\"/_next/static/chunks/04eq_ut3lda3~.js?dpl=dpl_BdwYag37Coka3wCmVQYgfikUc21G\",\"/_next/static/chunks/0.jffwitghhk6.js?dpl=dpl_BdwYag37Coka3wCmVQYgfikUc21G\",\"/_next/static/chunks/0b5wrdfrwab.k.js?dpl=dpl_BdwYag37Coka3wCmVQYgfikUc21G\",\"/_next/static/chunks/0i82lysj2jiv0.js?dpl=dpl_BdwYag37Coka3wCmVQYgfikUc21G\"],\"StyleCard\"]\n"])</script><script>self.__next_f.push([1,"38:[\"$\",\"section\",null,{\"className\":\"space-y-6\",\"children\":[[\"$\",\"h2\",null,{\"className\":\"font-heading text-xl font-semibold tracking-heading\",\"children\":\"More like this\"}],[\"$\",\"div\",null,{\"className\":\"grid gap-x-4 gap-y-6 grid-cols-1 sm:grid-cols-2\",\"children\":[[\"$\",\"$L3b\",\"3f2b79c1-d980-4380-a903-29856975fc37\",{\"style\":{\"id\":\"3f2b79c1-d980-4380-a903-29856975fc37\",\"url\":\"https://midday.ai\",\"siteName\":\"Midday\",\"screenshotUrl\":\"https://images.refero.design/styles/refero.design/image/5e426d8f-9d2c-4586-9b9d-29cbbff76648.jpg\",\"thumbnailUrl\":\"https://images.refero.design/styles/refero.design/image/a33c7b65-1bfc-4926-9c7a-5d0661894c90.jpg\",\"iconUrl\":null,\"previewVideoUrl\":\"https://images.refero.design/styles/refero.design/video/1333f37f-5032-4660-9fa5-d91ec9e1dba3.mp4\",\"previewVideoPosterUrl\":\"https://images.refero.design/styles/refero.design/image/324811a1-7d7b-4d6c-bd54-3f11e65e20bf.jpg\",\"previewVideoWidth\":1200,\"previewVideoHeight\":750,\"previewVideoDetailUrl\":\"https://images.refero.design/styles/refero.design/video/bbebffbe-8c27-4ced-bae3-b15f2dd4fe76.mp4\",\"previewVideoDetailPosterUrl\":\"https://images.refero.design/styles/refero.design/image/0ba618c2-8bbc-4e08-ba60-180bd4484a1e.jpg\",\"previewVideoDetailWidth\":1600,\"previewVideoDetailHeight\":1000,\"previewVideoDurationMs\":11640,\"colorScheme\":\"light\",\"colors\":[{\"name\":\"Parchment\",\"hex\":\"#dbdad7\",\"gradient\":\"$undefined\"},{\"name\":\"Paper\",\"hex\":\"#ffffff\",\"gradient\":\"$undefined\"},{\"name\":\"Sand\",\"hex\":\"#e6e4e0\",\"gradient\":\"$undefined\"},{\"name\":\"Ink\",\"hex\":\"#121212\",\"gradient\":\"$undefined\"},{\"name\":\"Smoke\",\"hex\":\"#616161\",\"gradient\":\"$undefined\"},{\"name\":\"Charcoal\",\"hex\":\"#18181b\",\"gradient\":\"$undefined\"}],\"fonts\":[\"Hedvig Letters Sans\",\"Hedvig Letters Serif\"],\"northStar\":\"Editorial broadsheet on parchment — a 72px serif headline over warm stone, spaced sans-serif body text, pill-shaped controls, zero shadows.\",\"managementSignals\":[],\"createdAt\":\"2026-04-30 00:04:36.281551\"},\"compact\":true}],[\"$\",\"$L3b\",\"3172cd4d-118a-4a16-a259-6b634d32322e\",{\"style\":{\"id\":\"3172cd4d-118a-4a16-a259-6b634d32322e\",\"url\":\"https://mercury.com\",\"siteName\":\"Mercury\",\"screenshotUrl\":\"https://images.refero.design/styles/refero.design/image/f5e7b964-aab6-4d9c-b1f6-96565ddde880.jpg\",\"thumbnailUrl\":\"https://images.refero.design/styles/refero.design/image/bf6a14ca-affd-4681-9b8a-a98f680fd7d1.jpg\",\"iconUrl\":\"https://images.refero.design/styles/refero.design/image/cebe9a93-1dc3-4b41-8456-f0ad9d316775.png\",\"previewVideoUrl\":\"https://images.refero.design/styles/refero.design/video/eb803ed8-c299-4423-87bc-61d1a41b88f2.mp4\",\"previewVideoPosterUrl\":\"https://images.refero.design/styles/refero.design/image/1e084062-4041-41dd-9a11-f439cd733af1.jpg\",\"previewVideoWidth\":1200,\"previewVideoHeight\":750,\"previewVideoDetailUrl\":\"https://images.refero.design/styles/refero.design/video/9a1861cd-385b-41a6-9d47-62239b2c8a0f.mp4\",\"previewVideoDetailPosterUrl\":\"https://images.refero.design/styles/refero.design/image/0ca7b304-01bd-43a7-b5a9-06f22714d05d.jpg\",\"previewVideoDetailWidth\":1600,\"previewVideoDetailHeight\":1000,\"previewVideoDurationMs\":41867,\"colorScheme\":\"dark\",\"colors\":[{\"name\":\"Onyx Canvas\",\"hex\":\"#171721\",\"gradient\":\"$undefined\"},{\"name\":\"Graphite Card\",\"hex\":\"#1e1e2a\",\"gradient\":\"$undefined\"},{\"name\":\"Obsidian Button\",\"hex\":\"#272735\",\"gradient\":\"$undefined\"},{\"name\":\"Slate Border\",\"hex\":\"#70707d\",\"gradient\":\"$undefined\"},{\"name\":\"Mist Border\",\"hex\":\"#e2e3ed\",\"gradient\":\"$undefined\"},{\"name\":\"Ash Text\",\"hex\":\"#c3c3cc\",\"gradient\":\"$undefined\"}],\"fonts\":[\"arcadia\",\"arcadiaDisplay\"],\"northStar\":\"Alpine banking at blue hour\",\"managementSignals\":[],\"createdAt\":\"2026-02-25 13:19:15\"},\"compact\":true}],[\"$\",\"$L3b\",\"46bca11b-6920-4d70-8dd7-c4e3dbc123c7\",{\"style\":{\"id\":\"46bca11b-6920-4d70-8dd7-c4e3dbc123c7\",\"url\":\"https://www.coinshift.xyz\",\"siteName\":\"iUSPC by Coinshift\",\"screenshotUrl\":\"https://images.refero.design/styles/refero.design/image/507a8a6e-c1b0-4eb3-b18c-690dfc500e64.jpg\",\"thumbnailUrl\":\"https://images.refero.design/styles/refero.design/image/d420c7a4-73c7-4001-8d33-c7f9a42fd600.jpg\",\"iconUrl\":\"https://images.refero.design/styles/refero.design/image/4ca4c361-e355-4a0c-a333-9126df7f63d6.png\",\"previewVideoUrl\":\"https://images.refero.design/styles/refero.design/video/02c934d6-8f82-4fb1-9ec8-914578291a4d.mp4\",\"previewVideoPosterUrl\":\"https://images.refero.design/styles/refero.design/image/179e15d8-343f-4388-81d6-97353ef3093e.jpg\",\"previewVideoWidth\":1200,\"previewVideoHeight\":750,\"previewVideoDetailUrl\":\"https://images.refero.design/styles/refero.design/video/787ee10c-8a4e-4e82-8398-f01d614aa719.mp4\",\"previewVideoDetailPosterUrl\":\"https://images.refero.design/styles/refero.design/image/b317f308-f4ed-4bab-9fa2-b41d2018d734.jpg\",\"previewVideoDetailWidth\":1600,\"previewVideoDetailHeight\":1000,\"previewVideoDurationMs\":16533,\"colorScheme\":\"dark\",\"colors\":[{\"name\":\"Abyss Ink\",\"hex\":\"#020617\",\"gradient\":\"$undefined\"},{\"name\":\"Deep Slate\",\"hex\":\"#0a0e1a\",\"gradient\":\"$undefined\"},{\"name\":\"Frost White\",\"hex\":\"#f1f5f9\",\"gradient\":\"$undefined\"},{\"name\":\"Cloud Gray\",\"hex\":\"#e5e7eb\",\"gradient\":\"$undefined\"},{\"name\":\"Slate Mist\",\"hex\":\"#64748b\",\"gradient\":\"$undefined\"},{\"name\":\"Graphite\",\"hex\":\"#475569\",\"gradient\":\"$undefined\"}],\"fonts\":[\"Inter\",\"ABCSynt\"],\"northStar\":\"Midnight trading floor — cold slate surfaces, a single ember pilot light, and grid lines drawn on darkness.\",\"managementSignals\":[],\"createdAt\":\"2026-05-07 18:55:36.23835\"},\"compact\":true}],\"$L3c\",\"$L3d\",\"$L3e\",\"$L3f\",\"$L40\",\"$L41\",\"$L42\",\"$L43\",\"$L44\",\"$L45\",\"$L46\",\"$L47\",\"$L48\",\"$L49\",\"$L4a\",\"$L4b\",\"$L4c\"]}]]}]\n"])</script><script>self.__next_f.push([1,"3c:[\"$\",\"$L3b\",\"b136f0a0-8064-4978-a18e-db54b9362c24\",{\"style\":{\"id\":\"b136f0a0-8064-4978-a18e-db54b9362c24\",\"url\":\"https://index.inc\",\"siteName\":\"Index\",\"screenshotUrl\":\"https://images.refero.design/styles/refero.design/image/d38f6f44-b935-469c-972b-5a54c23129c6.jpg\",\"thumbnailUrl\":\"https://images.refero.design/styles/refero.design/image/93b4f07b-db91-414f-a374-de08865e9de3.jpg\",\"iconUrl\":\"https://images.refero.design/styles/refero.design/image/78f0cb6d-7f6e-4add-832e-5c34c68009cd.png\",\"previewVideoUrl\":\"https://images.refero.design/styles/refero.design/video/1f60be18-084d-4ed7-9b77-58d9be7f5823.mp4\",\"previewVideoPosterUrl\":\"https://images.refero.design/styles/refero.design/image/2845a229-c125-41f8-9ec4-65d9489e05e9.jpg\",\"previewVideoWidth\":1200,\"previewVideoHeight\":750,\"previewVideoDetailUrl\":\"https://images.refero.design/styles/refero.design/video/c0a19641-29ed-443c-8248-f37827b7db68.mp4\",\"previewVideoDetailPosterUrl\":\"https://images.refero.design/styles/refero.design/image/81b39230-70fb-43e6-b17d-fe6080e37dc1.jpg\",\"previewVideoDetailWidth\":1600,\"previewVideoDetailHeight\":1000,\"previewVideoDurationMs\":12300,\"colorScheme\":\"dark\",\"colors\":[{\"name\":\"Abyss Black\",\"hex\":\"#02030b\",\"gradient\":\"$undefined\"},{\"name\":\"Midnight Indigo\",\"hex\":\"#04061c\",\"gradient\":\"$undefined\"},{\"name\":\"Slate Indigo\",\"hex\":\"#0c0a2b\",\"gradient\":\"$undefined\"},{\"name\":\"Carbon Iris\",\"hex\":\"#13151f\",\"gradient\":\"$undefined\"},{\"name\":\"Twilight Plum\",\"hex\":\"#2c2b52\",\"gradient\":\"$undefined\"},{\"name\":\"Iris Border\",\"hex\":\"#292a4d\",\"gradient\":\"$undefined\"}],\"fonts\":[\"Index\",\"Inter\",\"-apple-system\"],\"northStar\":\"twilight summit command center — a violet-tinted dark dashboard crowned by a single mountain horizon at dusk, where the only warm light is the coral CTA\",\"managementSignals\":[],\"createdAt\":\"2026-05-07 18:35:25.480535\"},\"compact\":true}]\n"])</script><script>self.__next_f.push([1,"3d:[\"$\",\"$L3b\",\"7c38e84b-aea0-4c8f-b3e9-60b994ee6c6b\",{\"style\":{\"id\":\"7c38e84b-aea0-4c8f-b3e9-60b994ee6c6b\",\"url\":\"https://www.slash.com\",\"siteName\":\"Slash\",\"screenshotUrl\":\"https://images.refero.design/styles/refero.design/image/c74df455-7532-4c5b-9433-358b96853adb.jpg\",\"thumbnailUrl\":\"https://images.refero.design/styles/refero.design/image/6b67b1a0-c73e-4a69-93e4-1df5e822cc73.jpg\",\"iconUrl\":\"https://images.refero.design/styles/refero.design/image/3d369f2c-f310-4dc2-ac55-c17c16831c34.png\",\"previewVideoUrl\":\"https://images.refero.design/styles/refero.design/video/c17ddacd-7083-4709-82d7-378ca0796a4a.mp4\",\"previewVideoPosterUrl\":\"https://images.refero.design/styles/refero.design/image/f51cd771-1bf7-4ea4-8510-f3a46d0f83cb.jpg\",\"previewVideoWidth\":1200,\"previewVideoHeight\":750,\"previewVideoDetailUrl\":\"https://images.refero.design/styles/refero.design/video/0af8133f-9c6c-42a2-95c7-fd4f62fe9f90.mp4\",\"previewVideoDetailPosterUrl\":\"https://images.refero.design/styles/refero.design/image/03cde3c7-03ac-4ca7-b853-df8b2bdfaae3.jpg\",\"previewVideoDetailWidth\":1600,\"previewVideoDetailHeight\":1000,\"previewVideoDurationMs\":29734,\"colorScheme\":\"dark\",\"colors\":[{\"name\":\"Obsidian\",\"hex\":\"#08080a\",\"gradient\":\"$undefined\"},{\"name\":\"Onyx\",\"hex\":\"#040406\",\"gradient\":\"$undefined\"},{\"name\":\"Carbon\",\"hex\":\"#121317\",\"gradient\":\"$undefined\"},{\"name\":\"Graphite\",\"hex\":\"#1c1d22\",\"gradient\":\"$undefined\"},{\"name\":\"Slate\",\"hex\":\"#2e3038\",\"gradient\":\"$undefined\"},{\"name\":\"Smoke\",\"hex\":\"#464853\",\"gradient\":\"$undefined\"}],\"fonts\":[\"Ivy Presto\",\"Inter\"],\"northStar\":\"Midnight vault with gilded ledger lines.\",\"managementSignals\":[],\"createdAt\":\"2026-04-30 00:26:09.009777\"},\"compact\":true}]\n"])</script><script>self.__next_f.push([1,"3e:[\"$\",\"$L3b\",\"573fe0d5-8f0b-4c59-bae3-3f2e67cc63f0\",{\"style\":{\"id\":\"573fe0d5-8f0b-4c59-bae3-3f2e67cc63f0\",\"url\":\"https://tableland.xyz\",\"siteName\":\"Tableland\",\"screenshotUrl\":\"https://images.refero.design/styles/refero.design/image/17fe0b6c-b4e6-4e5e-988f-d34f60f38bd4.jpg\",\"thumbnailUrl\":\"https://images.refero.design/styles/refero.design/image/c836092c-b995-43e8-b91c-ebca6543b1c5.jpg\",\"iconUrl\":\"https://images.refero.design/styles/refero.design/image/d40f14ca-bf5e-4d54-ae61-95ec2d8bc27d.png\",\"previewVideoUrl\":\"https://images.refero.design/styles/refero.design/video/828f96b8-b5d4-4fc0-94f7-f9597fa8d8e5.mp4\",\"previewVideoPosterUrl\":\"https://images.refero.design/styles/refero.design/image/ca9dc83e-bb96-44ae-8742-ef79c5bd99dc.jpg\",\"previewVideoWidth\":1200,\"previewVideoHeight\":750,\"previewVideoDetailUrl\":\"https://images.refero.design/styles/refero.design/video/4fa41e76-2fc5-4c18-a74c-72aee4a0a134.mp4\",\"previewVideoDetailPosterUrl\":\"https://images.refero.design/styles/refero.design/image/dd1e436a-01ba-4296-b6f4-eb52fa36af0d.jpg\",\"previewVideoDetailWidth\":1600,\"previewVideoDetailHeight\":1000,\"previewVideoDurationMs\":6967,\"colorScheme\":\"dark\",\"colors\":[{\"name\":\"Abyss Teal\",\"hex\":\"#75b6b5\",\"gradient\":\"$undefined\"},{\"name\":\"Mint Beacon\",\"hex\":\"#0be291\",\"gradient\":\"$undefined\"},{\"name\":\"Coral Ember\",\"hex\":\"#f4706b\",\"gradient\":\"$undefined\"},{\"name\":\"Lavender Mist\",\"hex\":\"#e4cbf2\",\"gradient\":\"$undefined\"},{\"name\":\"Void\",\"hex\":\"#101e1e\",\"gradient\":\"$undefined\"},{\"name\":\"Carbon\",\"hex\":\"#1a1a1a\",\"gradient\":\"$undefined\"}],\"fonts\":[\"Poppins\",\"monospace\"],\"northStar\":\"alpine dusk at the terminal — soft coral peaks rising over a deep green-black void with one mint-green signal light glowing on the horizon.\",\"managementSignals\":[],\"createdAt\":\"2026-05-07 18:07:14.632828\"},\"compact\":true}]\n"])</script><script>self.__next_f.push([1,"3f:[\"$\",\"$L3b\",\"c60f05ff-2420-4a24-92db-80c4b6a74683\",{\"style\":{\"id\":\"c60f05ff-2420-4a24-92db-80c4b6a74683\",\"url\":\"https://www.useorigin.com\",\"siteName\":\"Origin Financial\",\"screenshotUrl\":\"https://images.refero.design/styles/refero.design/image/2e3e242a-26b5-45c9-b63c-5048ee729f87.jpg\",\"thumbnailUrl\":\"https://images.refero.design/styles/refero.design/image/caa1bdad-fa0d-4b64-8c23-f0c5a9370a4a.jpg\",\"iconUrl\":\"https://images.refero.design/styles/refero.design/image/011ecfce-5760-469e-95b7-56ffc955bf2c.png\",\"previewVideoUrl\":\"https://images.refero.design/styles/refero.design/video/b2af7366-6d7f-41ac-8985-4356cd39a16e.mp4\",\"previewVideoPosterUrl\":\"https://images.refero.design/styles/refero.design/image/02d9c19b-b2e4-4d9a-805d-22ff505c31e0.jpg\",\"previewVideoWidth\":1200,\"previewVideoHeight\":750,\"previewVideoDetailUrl\":\"https://images.refero.design/styles/refero.design/video/0dd7172c-7a13-4948-ae4a-cf37640b6442.mp4\",\"previewVideoDetailPosterUrl\":\"https://images.refero.design/styles/refero.design/image/cb0a0caf-5094-4769-9447-8e34302fde76.jpg\",\"previewVideoDetailWidth\":1600,\"previewVideoDetailHeight\":1000,\"previewVideoDurationMs\":25050,\"colorScheme\":\"dark\",\"colors\":[{\"name\":\"Iris Gleam\",\"hex\":\"#847dff\",\"gradient\":\"$undefined\"},{\"name\":\"Cyan Signal\",\"hex\":\"#00b3dd\",\"gradient\":\"$undefined\"},{\"name\":\"Pale Iris\",\"hex\":\"#d1c9ff\",\"gradient\":\"$undefined\"},{\"name\":\"Deep Iris\",\"hex\":\"#4b49aa\",\"gradient\":\"$undefined\"},{\"name\":\"Orchid Bloom\",\"hex\":\"#dd90d8\",\"gradient\":\"$undefined\"},{\"name\":\"Periwinkle\",\"hex\":\"#90b8f0\",\"gradient\":\"$undefined\"}],\"fonts\":[\"Suisseintltrial\",\"Lyon Display\",\"Suisse Int'l\",\"Suisse Int'l Trial\",\"Roboto Mono\",\"Suisseintl\"],\"northStar\":\"midnight gallery of quiet wealth. A hushed, near-black room where oversized serif whispers and a few luminous color panels make finance feel like curated art.\",\"managementSignals\":[],\"createdAt\":\"2026-04-30 00:31:47.245225\"},\"compact\":true}]\n"])</script><script>self.__next_f.push([1,"40:[\"$\",\"$L3b\",\"a9941737-7a01-47b0-b187-df2bb16b27d8\",{\"style\":{\"id\":\"a9941737-7a01-47b0-b187-df2bb16b27d8\",\"url\":\"https://www.ai.work\",\"siteName\":\"Henry\",\"screenshotUrl\":\"https://images.refero.design/styles/refero.design/image/6d867c2e-5576-4d73-a110-93ad93c5de9d.jpg\",\"thumbnailUrl\":\"https://images.refero.design/styles/refero.design/image/18042cc9-6a26-499e-8130-1f754c919b16.jpg\",\"iconUrl\":\"https://images.refero.design/styles/refero.design/image/b7c7829d-f01c-4a7b-80c0-acdbef44bb49.png\",\"previewVideoUrl\":\"https://images.refero.design/styles/refero.design/video/b499c61b-91ed-4baf-a911-adb48628cc58.mp4\",\"previewVideoPosterUrl\":\"https://images.refero.design/styles/refero.design/image/fbb1c955-7ea6-482b-a737-08586c7eeb17.jpg\",\"previewVideoWidth\":1200,\"previewVideoHeight\":750,\"previewVideoDetailUrl\":\"https://images.refero.design/styles/refero.design/video/21c8f3b9-64e2-4f38-abfa-e39db1d24e85.mp4\",\"previewVideoDetailPosterUrl\":\"https://images.refero.design/styles/refero.design/image/f85c69f3-0d49-425d-a73f-db92152a72bb.jpg\",\"previewVideoDetailWidth\":1600,\"previewVideoDetailHeight\":1000,\"previewVideoDurationMs\":45134,\"colorScheme\":\"dark\",\"colors\":[{\"name\":\"Obsidian\",\"hex\":\"#000000\",\"gradient\":\"$undefined\"},{\"name\":\"Carbon\",\"hex\":\"#141414\",\"gradient\":\"$undefined\"},{\"name\":\"Tar\",\"hex\":\"#0c0c0c\",\"gradient\":\"$undefined\"},{\"name\":\"Bone\",\"hex\":\"#d4d0c9\",\"gradient\":\"$undefined\"},{\"name\":\"Ash\",\"hex\":\"#878581\",\"gradient\":\"$undefined\"},{\"name\":\"Smoke\",\"hex\":\"#615f5c\",\"gradient\":\"$undefined\"}],\"fonts\":[\"sans-serif\",\"NB International Pro\",\"NB International Pro Mono\",\"Inter\",\"NB International Pro Light\",\"NB International Pro Regular\",\"NB International Pro CG Medium\",\"NB International Pro CG Mono\"],\"northStar\":\"darkroom gallery at midnight — measured, restrained, photograph-centric\",\"managementSignals\":[],\"createdAt\":\"2026-05-10 22:31:28.810827\"},\"compact\":true}]\n"])</script><script>self.__next_f.push([1,"41:[\"$\",\"$L3b\",\"9cc537fc-97d8-4632-8703-f9aa296c2206\",{\"style\":{\"id\":\"9cc537fc-97d8-4632-8703-f9aa296c2206\",\"url\":\"https://eco.com\",\"siteName\":\"Eco\",\"screenshotUrl\":\"https://images.refero.design/styles/refero.design/image/5c5e565b-80c3-49d7-b429-c10c2a7de134.jpg\",\"thumbnailUrl\":\"https://images.refero.design/styles/refero.design/image/a61620f4-4648-487d-9ae9-5576e38069a7.jpg\",\"iconUrl\":null,\"previewVideoUrl\":\"https://images.refero.design/styles/refero.design/video/aba14586-387b-4e69-9f3a-381704278e50.mp4\",\"previewVideoPosterUrl\":\"https://images.refero.design/styles/refero.design/image/f2e7c319-6049-43cf-8b9f-79f4c528c37c.jpg\",\"previewVideoWidth\":1200,\"previewVideoHeight\":750,\"previewVideoDetailUrl\":\"https://images.refero.design/styles/refero.design/video/15b49c44-867d-4ea7-b798-f684bd4c972c.mp4\",\"previewVideoDetailPosterUrl\":\"https://images.refero.design/styles/refero.design/image/b6cb9bab-9890-4027-8842-9b04748b2ad4.jpg\",\"previewVideoDetailWidth\":1600,\"previewVideoDetailHeight\":1000,\"previewVideoDurationMs\":19960,\"colorScheme\":\"both\",\"colors\":[{\"name\":\"Bone\",\"hex\":\"#ffffff\",\"gradient\":\"$undefined\"},{\"name\":\"Ash Mist\",\"hex\":\"#efefef\",\"gradient\":\"$undefined\"},{\"name\":\"Vault Ink\",\"hex\":\"#0f111a\",\"gradient\":\"$undefined\"},{\"name\":\"Absolute\",\"hex\":\"#000000\",\"gradient\":\"$undefined\"},{\"name\":\"Carbon\",\"hex\":\"#141414\",\"gradient\":\"$undefined\"},{\"name\":\"Charcoal\",\"hex\":\"#2a2a2a\",\"gradient\":\"$undefined\"}],\"fonts\":[\"Interdisplay\",\"Roobert\",\"Inter 24 Pt\",\"Fragmentmono\",\"Aeonik Mono\"],\"northStar\":\"skyline vault at dusk — a near-monochrome ledger where negative space and oversized display type carry the entire brand weight, interrupted only by tiny electric-blue marks.\",\"managementSignals\":[],\"createdAt\":\"2026-01-18 17:11:39\"},\"compact\":true}]\n"])</script><script>self.__next_f.push([1,"42:[\"$\",\"$L3b\",\"850ee61c-4ecd-4558-9c0c-fab99721b34c\",{\"style\":{\"id\":\"850ee61c-4ecd-4558-9c0c-fab99721b34c\",\"url\":\"https://www.11x.ai\",\"siteName\":\"11x– Digital workers\",\"screenshotUrl\":\"https://images.refero.design/styles/refero.design/image/23125314-fa1e-43e2-9f82-c4363f05dfd2.jpg\",\"thumbnailUrl\":\"https://images.refero.design/styles/refero.design/image/d7c7c3c0-b0ef-49ff-9b4a-8a31c6c635cf.jpg\",\"iconUrl\":\"https://images.refero.design/styles/refero.design/image/eddf3bb0-a890-4001-a7c6-859f1c18cbc7.png\",\"previewVideoUrl\":\"https://images.refero.design/styles/refero.design/video/231d1a76-3deb-48a3-8dab-9c2e35e9f315.mp4\",\"previewVideoPosterUrl\":\"https://images.refero.design/styles/refero.design/image/a86e8922-d7cc-42ec-ac58-4be871419c9e.jpg\",\"previewVideoWidth\":1200,\"previewVideoHeight\":750,\"previewVideoDetailUrl\":\"https://images.refero.design/styles/refero.design/video/3cff58d0-93f4-472a-8cf3-222591d137db.mp4\",\"previewVideoDetailPosterUrl\":\"https://images.refero.design/styles/refero.design/image/bdd420ad-11f5-46f7-b18d-652c16a4879d.jpg\",\"previewVideoDetailWidth\":1600,\"previewVideoDetailHeight\":1000,\"previewVideoDurationMs\":22867,\"colorScheme\":\"both\",\"colors\":[{\"name\":\"Obsidian\",\"hex\":\"#000000\",\"gradient\":\"$undefined\"},{\"name\":\"Paper White\",\"hex\":\"#ffffff\",\"gradient\":\"$undefined\"},{\"name\":\"Deep Teal\",\"hex\":\"#0b252a\",\"gradient\":\"$undefined\"},{\"name\":\"Bone\",\"hex\":\"#f6f5f5\",\"gradient\":\"$undefined\"},{\"name\":\"Sandstone\",\"hex\":\"#f5ece5\",\"gradient\":\"$undefined\"},{\"name\":\"Ash Blush\",\"hex\":\"#ede2d7\",\"gradient\":\"$undefined\"}],\"fonts\":[\"ES Allianz\"],\"northStar\":\"Cinematic editorial desert — full-bleed terrain photography against monumental serif headlines, where the page reads like a luxury magazine spread.\",\"managementSignals\":[],\"createdAt\":\"2026-05-08 18:56:28.795579\"},\"compact\":true}]\n"])</script><script>self.__next_f.push([1,"43:[\"$\",\"$L3b\",\"eeeb6ac9-fc07-4965-935a-e1989ed831f1\",{\"style\":{\"id\":\"eeeb6ac9-fc07-4965-935a-e1989ed831f1\",\"url\":\"https://www.default.com\",\"siteName\":\"Default\",\"screenshotUrl\":\"https://images.refero.design/styles/refero.design/image/6977c928-f98b-4ef0-90ff-030b0286a775.jpg\",\"thumbnailUrl\":\"https://images.refero.design/styles/refero.design/image/6c8c0b69-855e-49e5-87eb-0be1b675c232.jpg\",\"iconUrl\":\"https://images.refero.design/styles/refero.design/image/3853782f-bc2f-4c19-846a-fa5ef09290fa.png\",\"previewVideoUrl\":\"https://images.refero.design/styles/refero.design/video/b71d95ec-7b69-428a-b87e-8e32e50dff4a.mp4\",\"previewVideoPosterUrl\":\"https://images.refero.design/styles/refero.design/image/38addea5-afe5-4cdd-804e-384cbf72c359.jpg\",\"previewVideoWidth\":1200,\"previewVideoHeight\":750,\"previewVideoDetailUrl\":\"https://images.refero.design/styles/refero.design/video/d92c8b89-ddf0-4422-bd1d-5f30c6a7dac1.mp4\",\"previewVideoDetailPosterUrl\":\"https://images.refero.design/styles/refero.design/image/ff619359-489f-475e-a2ea-90bf4c4c092a.jpg\",\"previewVideoDetailWidth\":1600,\"previewVideoDetailHeight\":1000,\"previewVideoDurationMs\":17850,\"colorScheme\":\"dark\",\"colors\":[{\"name\":\"Void\",\"hex\":\"#0b0c0e\",\"gradient\":\"$undefined\"},{\"name\":\"Graphite\",\"hex\":\"#131416\",\"gradient\":\"$undefined\"},{\"name\":\"Charcoal\",\"hex\":\"#1f1f21\",\"gradient\":\"$undefined\"},{\"name\":\"Smoke\",\"hex\":\"#3c3d3e\",\"gradient\":\"$undefined\"},{\"name\":\"Steel\",\"hex\":\"#71717a\",\"gradient\":\"$undefined\"},{\"name\":\"Fog\",\"hex\":\"#858687\",\"gradient\":\"$undefined\"}],\"fonts\":[\"Inter\"],\"northStar\":\"Mission control behind frosted glass — weight 400 headlines float over matte-black panels lit by thin blue ring-light accents.\",\"managementSignals\":[],\"createdAt\":\"2026-05-07 18:20:28.470026\"},\"compact\":true}]\n"])</script><script>self.__next_f.push([1,"44:[\"$\",\"$L3b\",\"c75603c7-492d-4c26-9744-9acc22fe6225\",{\"style\":{\"id\":\"c75603c7-492d-4c26-9744-9acc22fe6225\",\"url\":\"https://www.angellist.com\",\"siteName\":\"AngelList\",\"screenshotUrl\":\"https://images.refero.design/styles/refero.design/image/73a1c285-e9f6-4415-89db-b5c4d5315722.jpg\",\"thumbnailUrl\":\"https://images.refero.design/styles/refero.design/image/36112875-29f9-4f28-8550-35b25b5511c3.jpg\",\"iconUrl\":null,\"previewVideoUrl\":\"https://images.refero.design/styles/refero.design/video/6f8e4c77-6765-49db-b081-d0046c4d9c00.mp4\",\"previewVideoPosterUrl\":\"https://images.refero.design/styles/refero.design/image/4069d02a-d165-4111-87ba-9c7392b97466.jpg\",\"previewVideoWidth\":1200,\"previewVideoHeight\":750,\"previewVideoDetailUrl\":\"https://images.refero.design/styles/refero.design/video/45d82ca0-b44a-4302-9750-f99a24d54fab.mp4\",\"previewVideoDetailPosterUrl\":\"https://images.refero.design/styles/refero.design/image/6572945d-9e2f-453a-b4aa-fb7676a00f2b.jpg\",\"previewVideoDetailWidth\":1600,\"previewVideoDetailHeight\":1000,\"previewVideoDurationMs\":14450,\"colorScheme\":\"dark\",\"colors\":[{\"name\":\"Abyssal Teal\",\"hex\":\"#001d21\",\"gradient\":\"$undefined\"},{\"name\":\"Deep Reef\",\"hex\":\"#002b31\",\"gradient\":\"$undefined\"},{\"name\":\"Bio Mint\",\"hex\":\"#e0fee6\",\"gradient\":\"$undefined\"},{\"name\":\"Lavender Dawn\",\"hex\":\"#cdcbff\",\"gradient\":\"$undefined\"},{\"name\":\"Vivid Iris\",\"hex\":\"#3a25f5\",\"gradient\":\"$undefined\"},{\"name\":\"Pale Periwinkle\",\"hex\":\"#bdbbff\",\"gradient\":\"$undefined\"}],\"fonts\":[\"angellistDisplay\",\"angellist\"],\"northSt