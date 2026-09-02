# Monad — Style Reference
> editorial tech journal on warm parchment

**Theme:** light

Monad renders its entire interface on a warm parchment canvas (#f6f3f1) that immediately separates it from the typical pure-white SaaS template. Headlines carry editorial weight in Untitled Serif at weight 400 — never bold — while every body, nav, and UI string runs in ABC Diatype Mono, giving the site the texture of a technical manual typeset for a literary magazine. A single vivid Lake Blue (#2b59d1) is the only chromatic accent for primary actions; everything else lives in a warm grayscale, so a periwinkle card surface (#cfdaf5) and soft pastel gradient washes (coral, sky, mint, gold) read as deliberate punctuation rather than noise. Components lean on hairline borders and 100px pill containers rather than shadows, and the rhythm stays calm and spacious with 40px card padding and generous vertical breathing room between sections.

## Tokens — Colors

| Name | Value | Token | Role |
|------|-------|-------|------|
| Parchment | `#f6f3f1` | `--color-parchment` | Page canvas and the majority of surface fills — this warm off-white IS the brand's signature surface, immediately distinguishing the site from pure-white SaaS templates |
| Lake Blue | `#2b59d1` | `--color-lake-blue` | Violet wash for highlight backgrounds, decorative bands, and soft emphasis behind content. Do not promote it to the primary CTA color |
| Periwinkle Mist | `#cfdaf5` | `--color-periwinkle-mist` | Muted UI surface for disabled controls, low-emphasis panels, and placeholder blocks. |
| Sky Blue | `#a0b5eb` | `--color-sky-blue` | Decorative gradient stop — appears in atmospheric washes and the pipeline diagram's flow lines, never as a UI fill |
| Mint | `#a7fccd` | `--color-mint` | Supporting palette color for small decorative accents when the core palette needs contrast. |
| Coral | `#ff9473` | `--color-coral` | Supporting palette color for small decorative accents when the core palette needs contrast. |
| Gold | `#ecda98` | `--color-gold` | Decorative gradient stop — warm accent in gradient washes, never used in functional UI |
| Crimson | `#f37a0a` | `--color-crimson` | Decorative gradient stop — deep warm tone in gradient washes alongside gold and coral |
| Off-Black | `#242424` | `--color-off-black` | High-contrast neutral action fill for primary buttons on light surfaces. |
| Ink | `#000000` | `--color-ink` | Announcement bar surface and certain heading fills — the black band at the top of the page and select heading contexts |
| Graphite | `#4e4d4d` | `--color-graphite` | Secondary text — body copy and sub-headings that need less weight than primary headlines |
| Smoke | `#797776` | `--color-smoke` | Muted helper text and tertiary links |
| Ash | `#cecac8` | `--color-ash` | Hairline borders — 1px solid lines separating sections, outlining pipeline diagram nodes, and defining card edges |

## Tokens — Typography

### ABC Diatype Mono — Body text, navigation, buttons, badges, tags, and ALL UI strings. The monospace choice across every functional element gives the interface its technical-manual character — body copy at 16-20px reads as data, not marketing. Nav labels and badges use 18px uppercase with tighter tracking; small print and meta text use 12px uppercase. Weight 500 is reserved for emphasized UI labels. · `--font-abc-diatype-mono`
- **Substitute:** JetBrains Mono, IBM Plex Mono, or Space Mono
- **Weights:** 400, 500
- **Sizes:** 12px, 14px, 16px, 18px, 20px, 28px
- **Line height:** 1.0–1.35 (varies by size)
- **Letter spacing:** -0.033em at 12px, -0.025em at 16px, -0.022em at 18px, -0.02em at 14px and 20px, -0.014em at 28px
- **Role:** Body text, navigation, buttons, badges, tags, and ALL UI strings. The monospace choice across every functional element gives the interface its technical-manual character — body copy at 16-20px reads as data, not marketing. Nav labels and badges use 18px uppercase with tighter tracking; small print and meta text use 12px uppercase. Weight 500 is reserved for emphasized UI labels.

### Untitled Serif — Display and heading type only — used at 80px (hero), 48px (section), 40px and 32px (sub-section), 24px (feature card titles). Weight is locked at 400 across all sizes; the serif's natural contrast and the -0.02em letter-spacing do the heavy lifting instead of bold weight. This is the editorial confidence signature: headlines whisper through typographic refinement rather than shout through weight. · `--font-untitled-serif`
- **Substitute:** Times New Roman, Georgia, or any editorial serif with similar stroke contrast
- **Weights:** 400
- **Sizes:** 24px, 32px, 40px, 48px, 80px
- **Line height:** 1.2
- **Letter spacing:** -0.02em at all sizes (-1.6px at 80px, -0.96px at 48px, -0.8px at 40px, -0.64px at 32px, -0.48px at 24px)
- **Role:** Display and heading type only — used at 80px (hero), 48px (section), 40px and 32px (sub-section), 24px (feature card titles). Weight is locked at 400 across all sizes; the serif's natural contrast and the -0.02em letter-spacing do the heavy lifting instead of bold weight. This is the editorial confidence signature: headlines whisper through typographic refinement rather than shout through weight.

### Untitled Sans — Untitled Sans — detected in extracted data but not described by AI · `--font-untitled-sans`
- **Weights:** 400
- **Sizes:** 16px
- **Line height:** 1.35
- **Letter spacing:** -0.02
- **Role:** Untitled Sans — detected in extracted data but not described by AI

### Type Scale

| Role | Size | Line Height | Letter Spacing | Token |
|------|------|-------------|----------------|-------|
| caption | 12px | 1.2 | -0.4px | `--text-caption` |
| body-sm | 14px | 1.35 | -0.28px | `--text-body-sm` |
| body | 16px | 1.35 | -0.4px | `--text-body` |
| label | 18px | 1.2 | -0.4px | `--text-label` |
| body-lg | 20px | 1.35 | -0.4px | `--text-body-lg` |
| subheading | 24px | 1.2 | -0.48px | `--text-subheading` |
| heading-sm | 32px | 1.2 | -0.64px | `--text-heading-sm` |
| heading | 40px | 1.2 | -0.8px | `--text-heading` |
| heading-lg | 48px | 1.2 | -0.96px | `--text-heading-lg` |
| display | 80px | 1.2 | -1.6px | `--text-display` |

## Tokens — Spacing & Shapes

**Base unit:** 8px

**Density:** comfortable

### Spacing Scale

| Name | Value | Token |
|------|-------|-------|
| 8 | 8px | `--spacing-8` |
| 16 | 16px | `--spacing-16` |
| 24 | 24px | `--spacing-24` |
| 32 | 32px | `--spacing-32` |
| 40 | 40px | `--spacing-40` |
| 64 | 64px | `--spacing-64` |
| 72 | 72px | `--spacing-72` |
| 80 | 80px | `--spacing-80` |
| 200 | 200px | `--spacing-200` |
| 216 | 216px | `--spacing-216` |

### Border Radius

| Element | Value |
|---------|-------|
| tags | 9999px |
| cards | 40px |
| pills | 9999px |
| buttons | 100px |

### Shadows

| Name | Value | Token |
|------|-------|-------|
| md | `rgba(0, 0, 0, 0.1) 0px 0px 10px 0px` | `--shadow-md` |

### Layout

- **Page max-width:** 1432px
- **Section gap:** 64px
- **Card padding:** 40px
- **Element gap:** 16px

## Components

### Announcement Bar
**Role:** Top-of-page notification strip

Full-width black (#000000) bar, ~40px tall, containing mono text in white (#f6f3f1) at 14px and a small white pill button (9999px radius, white border, 12px uppercase text) anchored right. Close icon (×) in white at far right.

### Primary Pill Button (Blue)
**Role:** Primary conversion action

Lake Blue (#2b59d1) fill, white text in ABC Diatype Mono at 14px uppercase, 100px border-radius, 16px 32px padding, with a trailing arrow (▸) glyph in white. Height ~48px. This is the only saturated fill in the system.

### Primary Pill Button (Black)
**Role:** Secondary conversion action

Off-Black (#242424) fill, white text in ABC Diatype Mono at 14px uppercase, 100px border-radius, 16px 32px padding, no arrow. Height ~48px.

### Ghost Pill Button
**Role:** Tertiary navigation action

Transparent fill, 1px Off-Black (#242424) border, Off-Black text in ABC Diatype Mono at 14px uppercase, 100px border-radius, 16px 32px padding. Height ~48px.

### Text Link with Arrow
**Role:** Navigation link with directional indicator

Transparent fill, Off-Black (#242424) text in ABC Diatype Mono at 14px, trailing rightward arrow (→) in Off-Black. No background or border. Uppercase tracking.

### Pipeline Node Tag
**Role:** Labeled node in the data pipeline diagram

Parchment (#f6f3f1) fill, 1px Ash (#cecac8) border, 9999px border-radius (full pill), small mono icon (12px) + 14px mono uppercase text, 12px 20px padding. Connected by thin curved Ash lines to adjacent nodes.

### Feature Card
**Role:** Product capability card with icon, title, description

Transparent or Parchment fill, 1px Ash (#cecac8) border, 40px border-radius, 40px padding. Small mono icon (20px) in top-left at 16px padding offset. Title in Untitled Serif at 24px weight 400, Off-Black. Body in ABC Diatype Mono at 16px weight 400, Graphite (#4e4d4d). No shadow.

### Elevated Feature Card (Periwinkle)
**Role:** Hero feature card with gradient illustration

Periwinkle Mist (#cfdaf5) fill, 40px border-radius, 40px padding. Contains a large gradient illustration on the right side using Coral → Sky Blue → Mint washes. Title in Untitled Serif 24px, body in mono 16px. This is the one card that uses a colored surface to draw the eye.

### FAQ Accordion Item
**Role:** Expandable question/answer row

Full-width row, 40px vertical padding, 1px Ash (#cecac8) bottom border (no top border). Question text in Untitled Serif at 24px weight 400, Off-Black. Trailing chevron icon (↓) in Off-Black, 20px, right-aligned. No background fill change on hover.

### Logo Strip
**Role:** Social proof partner logo row

Single horizontal row of 6-7 partner logos in grayscale (desaturated from original brand colors), evenly spaced with ~32px gaps, left-aligned within max-width container. No logo lockup borders or cards.

### Gradient Atmospheric Wash
**Role:** Decorative background gradient blob

Large blurred radial/linear gradient using Coral (#ff9473 80% opacity) → Sky Blue (#a0b5eb 80% opacity) or Sky Blue → Mint (#a7fccd), rendered with blur(50-75px) filter, positioned behind hero or feature content. Never sharp-edged, always softly diffused.

### Navigation Bar
**Role:** Primary site navigation

Transparent or Parchment background, logo on far left (monad wordmark + circular dot mark), 4-5 nav text links centered or left-grouped in ABC Diatype Mono 18px uppercase Off-Black, action buttons (Login ghost + Get a Demo blue pill) right-aligned. ~80px height, no visible border.

### Hero Section
**Role:** First-screen headline and subtext

Full-width Parchment background, centered content stack: Untitled Serif headline at 80px weight 400 Off-Black, monospace subtext at 20px Graphite (#4e4d4d) at 1.35 line-height, two pill buttons centered below. No background image — pure typographic hero.

## Do's and Don'ts

### Do
- Use Untitled Serif at weight 400 for all headings — never go bold; the serif's stroke contrast and -0.02em tracking carry the weight visually
- Use ABC Diatype Mono for all body copy, buttons, nav labels, badges, and functional UI text — the monospace IS the brand voice
- Set all button and tag border-radius to 100px or 9999px — pill shapes are the container language of this system
- Use Parchment (#f6f3f1) as the page canvas — never substitute pure white (#ffffff); the warm tint is signature
- Reserve Lake Blue (#2b59d1) exclusively for the single primary action per screen; all other buttons use Off-Black or ghost variants
- Use 1px solid Ash (#cecac8) for all borders and dividers — avoid thicker weights or darker border colors
- Apply uppercase + tight tracking to all nav labels, buttons, and tag text via the monospace family

### Don't
- Never set headings in bold or 600+ weight — Untitled Serif headlines stay at 400 across all sizes
- Never use pure white (#ffffff) as a page background — always use Parchment (#f6f3f1) to preserve the warm surface
- Never use Lake Blue (#2b59d1) for anything other than the single primary action fill — it loses meaning if scattered
- Never substitute a sans-serif for the monospace body font — the mono/serif pairing is the defining typographic gesture
- Never apply drop shadows to cards — use 1px Ash borders and surface color contrast (Parchment → Periwinkle) for elevation instead
- Never use corner radii below 16px on cards or below 100px on buttons — the system is pill-and-soft-rect, never sharp
- Never introduce additional accent colors for UI elements — the pastel palette (Sky, Mint, Coral, Gold) is decorative-only and belongs in illustrations and gradient washes

## Surfaces

| Level | Name | Value | Purpose |
|-------|------|-------|---------|
| 1 | Parchment | `#f6f3f1` | Page canvas — the base warm off-white that fills the entire viewport |
| 2 | Periwinkle Mist | `#cfdaf5` | Elevated card surface — the one colored card that breaks the monochrome to draw the eye |
| 3 | Off-Black | `#242424` | Dark surface for secondary buttons and inverted UI contexts |
| 4 | Ink | `#000000` | Announcement bar — the darkest surface, used for the top notification strip |

## Elevation

- **Subtle ambient elevation:** `rgba(0, 0, 0, 0.1) 0px 0px 10px 0px`

## Imagery

The visual language is dominated by a custom data pipeline diagram: pill-shaped bordered nodes connected by thin curved lines, with small icons inside each node representing data sources (Any Source, Cloud Logs, Vulnerabilities) and destinations (SIEM, Cloud Storage, Data Lake). The diagram uses a soft green radial glow at the center hub to suggest data normalization. Gradient atmospheric washes (Coral → Sky Blue, Sky Blue → Mint) with heavy blur filters create soft color halos behind hero and feature content. Partner logos appear desaturated in a single social-proof row. The 'In-flight Data Transforms' card features a large gradient illustration with overlapping translucent geometric shapes. No photography is used — the brand communicates through typography, diagram, and color wash alone.

## Agent Prompt Guide

Quick Color Reference:
- text: #242424 (Off-Black)
- background: #f6f3f1 (Parchment)
- border: #cecac8 (Ash)
- accent: #2b59d1 (Lake Blue)
- primary action: no distinct CTA color

Example Component Prompts:

1. Create a hero section on Parchment (#f6f3f1) background. Centered headline in Untitled Serif at 80px weight 400, color #242424, letter-spacing -1.6px. Subtext below in ABC Diatype Mono at 20px weight 400, color #4e4d4d, line-height 1.35. Two centered pill buttons: primary Lake Blue (#2b59d1) with white text, and ghost (1px #242424 border, transparent fill, #242424 text), both 100px border-radius, 16px 32px padding, ABC Diatype Mono 14px uppercase.

2. Create a feature card on Parchment background. 1px solid #cecac8 border, 40px border-radius, 40px padding. Small 20px mono icon top-left at #242424. Title in Untitled Serif 24px weight 400, #242424. Body in ABC Diatype Mono 16px weight 400, #4e4d4d. No shadow.

3. Create a secondary pill button: Off-Black (#242424) fill, white text in ABC Diatype Mono 14px uppercase, 100px border-radius, 16px 32px padding, no arrow.

4. Create an FAQ accordion row: full-width, 40px vertical padding, 1px solid #cecac8 bottom border only. Question in Untitled Serif 24px weight 400, #242424. Trailing down-chevron icon (↓) in #242424 at 20px, right-aligned. No background fill.

5. Create a pipeline diagram node tag: Parchment (#f6f3f1) fill, 1px solid #cecac8 border, 9999px border-radius, 12px 20px padding. Small 12px icon + 14px text in ABC Diatype Mono uppercase, #242424.

## Typography Pairing Philosophy

The serif-mono pairing is the single most distinctive design choice in this system. Untitled Serif handles all hierarchical display text (headlines, section titles, feature card titles, FAQ questions) — it carries editorial authority through its stroke contrast and refined letterforms, not through weight (always 400). ABC Diatype Mono handles everything functional: body paragraphs, navigation, button labels, badges, tags, and inline UI text. This creates a consistent voice: the serif announces, the mono instructs. A page that swapped in a sans-serif for body would lose its identity immediately.

## Similar Brands

- **Linear** — Shares the restrained monochrome palette and minimal-elevation card approach, though Monad's warm Parchment canvas and serif headlines set it apart from Linear's cooler white surface
- **Stripe** — Both use custom editorial serif typefaces for headlines with tight letter-spacing and -0.02em tracking, treating the homepage as a typographic composition rather than a product screenshot
- **Vercel** — Shares the comfortable-density spacing, generous section gaps, and pill-shaped button language, though Monad adds the warm canvas and mono body twist
- **Railway** — Both target developer audiences with a monospace-leaning UI vocabulary and minimal decoration, but Monad layers in the editorial serif for a more literary feel
- **Arc Browser** — Both use warm off-white surfaces rather than pure white, and both treat the page as a designed editorial artifact rather than a typical SaaS template

## Quick Start

### CSS Custom Properties

```css
:root {
  /* Colors */
  --color-parchment: #f6f3f1;
  --color-lake-blue: #2b59d1;
  --color-periwinkle-mist: #cfdaf5;
  --color-sky-blue: #a0b5eb;
  --color-mint: #a7fccd;
  --color-coral: #ff9473;
  --color-gold: #ecda98;
  --color-crimson: #f37a0a;
  --color-off-black: #242424;
  --color-ink: #000000;
  --color-graphite: #4e4d4d;
  --color-smoke: #797776;
  --color-ash: #cecac8;

  /* Typography — Font Families */
  --font-abc-diatype-mono: 'ABC Diatype Mono', ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, monospace;
  --font-untitled-serif: 'Untitled Serif', ui-serif, Georgia, Cambria, "Times New Roman", Times, serif;
  --font-untitled-sans: 'Untitled Sans', ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;

  /* Typography — Scale */
  --text-caption: 12px;
  --leading-caption: 1.2;
  --tracking-caption: -0.4px;
  --text-body-sm: 14px;
  --leading-body-sm: 1.35;
  --tracking-body-sm: -0.28px;
  --text-body: 16px;
  --leading-body: 1.35;
  --tracking-body: -0.4px;
  --text-label: 18px;
  --leading-label: 1.2;
  --tracking-label: -0.4px;
  --text-body-lg: 20px;
  --leading-body-lg: 1.35;
  --tracking-body-lg: -0.4px;
  --text-subheading: 24px;
  --leading-subheading: 1.2;
  --tracking-subheading: -0.48px;
  --text-heading-sm: 32px;
  --leading-heading-sm: 1.2;
  --tracking-heading-sm: -0.64px;
  --text-heading: 40px;
  --leading-heading: 1.2;
  --tracking-heading: -0.8px;
  --text-heading-lg: 48px;
  --leading-heading-lg: 1.2;
  --tracking-heading-lg: -0.96px;
  --text-display: 80px;
  --leading-display: 1.2;
  --tracking-display: -1.6px;

  /* Typography — Weights */
  --font-weight-regular: 400;
  --font-weight-medium: 500;

  /* Spacing */
  --spacing-unit: 8px;
  --spacing-8: 8px;
  --spacing-16: 16px;
  --spacing-24: 24px;
  --spacing-32: 32px;
  --spacing-40: 40px;
  --spacing-64: 64px;
  --spacing-72: 72px;
  --spacing-80: 80px;
  --spacing-200: 200px;
  --spacing-216: 216px;

  /* Layout */
  --page-max-width: 1432px;
  --section-gap: 64px;
  --card-padding: 40px;
  --element-gap: 16px;

  /* Border Radius */
  --radius-2xl: 16px;
  --radius-3xl: 40px;
  --radius-full: 100px;
  --radius-full-2: 2000px;
  --radius-full-3: 9999px;

  /* Named Radii */
  --radius-tags: 9999px;
  --radius-cards: 40px;
  --radius-pills: 9999px;
  --radius-buttons: 100px;

  /* Shadows */
  --shadow-md: rgba(0, 0, 0, 0.1) 0px 0px 10px 0px;

  /* Surfaces */
  --surface-parchment: #f6f3f1;
  --surface-periwinkle-mist: #cfdaf5;
  --surface-off-black: #242424;
  --surface-ink: #000000;
}
```

### Tailwind v4

```css
@theme {
  /* Colors */
  --color-parchment: #f6f3f1;
  --color-lake-blue: #2b59d1;
  --color-periwinkle-mist: #cfdaf5;
  --color-sky-blue: #a0b5eb;
  --color-mint: #a7fccd;
  --color-coral: #ff9473;
  --color-gold: #ecda98;
  --color-crimson: #f37a0a;
  --color-off-black: #242424;
  --color-ink: #000000;
  --color-graphite: #4e4d4d;
  --color-smoke: #797776;
  --color-ash: #cecac8;

  /* Typography */
  --font-abc-diatype-mono: 'ABC Diatype Mono', ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, monospace;
  --font-untitled-serif: 'Untitled Serif', ui-serif, Georgia, Cambria, "Times New Roman", Times, serif;
  --font-untitled-sans: 'Untitled Sans', ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;

  /* Typography — Scale */
  --text-caption: 12px;
  --leading-caption: 1.2;
  --tracking-caption: -0.4px;
  --text-body-sm: 14px;
  --leading-body-sm: 1.35;
  --tracking-body-sm: -0.28px;
  --text-body: 16px;
  --leading-body: 1.35;
  --tracking-body: -0.4px;
  --text-label: 18px;
  --leading-label: 1.2;
  --tracking-label: -0.4px;
  --text-body-lg: 20px;
  --leading-body-lg: 1.35;
  --tracking-body-lg: -0.4px;
  --text-subheading: 24px;
  --leading-subheading: 1.2;
  --tracking-subheading: -0.48px;
  --text-heading-sm: 32px;
  --leading-heading-sm: 1.2;
  --tracking-heading-sm: -0.64px;
  --text-heading: 40px;
  --leading-heading: 1.2;
  --tracking-heading: -0.8px;
  --text-heading-lg: 48px;
  --leading-heading-lg: 1.2;
  --tracking-heading-lg: -0.96px;
  --text-display: 80px;
  --leading-display: 1.2;
  --tracking-display: -1.6px;

  /* Spacing */
  --spacing-8: 8px;
  --spacing-16: 16px;
  --spacing-24: 24px;
  --spacing-32: 32px;
  --spacing-40: 40px;
  --spacing-64: 64px;
  --spacing-72: 72px;
  --spacing-80: 80px;
  --spacing-200: 200px;
  --spacing-216: 216px;

  /* Border Radius */
  --radius-2xl: 16px;
  --radius-3xl: 40px;
  --radius-full: 100px;
  --radius-full-2: 2000px;
  --radius-full-3: 9999px;

  /* Shadows */
  --shadow-md: rgba(0, 0, 0, 0.1) 0px 0px 10px 0px;
}
```
</code></pre></div></div></div></div></div></main></div><script>$RS=function(a,b){a=document.getElementById(a);b=document.getElementById(b);for(a.parentNode.removeChild(a);a.firstChild;)b.parentNode.insertBefore(a.firstChild,b);b.parentNode.removeChild(b)};$RS("S:2","P:2")</script><div hidden id="S:4"><li class="flex items-start gap-2 text-sm text-foreground"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-x mt-0.5 size-4 shrink-0 text-red-500" aria-hidden="true"><path d="M18 6 6 18"></path><path d="m6 6 12 12"></path></svg><span>Never substitute a sans-serif for the monospace body font — the mono/serif pairing is the defining typographic gesture</span></li></div><script>$RS("S:4","P:4")</script><div hidden id="S:5"><li class="flex items-start gap-2 text-sm text-foreground"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-x mt-0.5 size-4 shrink-0 text-red-500" aria-hidden="true"><path d="M18 6 6 18"></path><path d="m6 6 12 12"></path></svg><span>Never apply drop shadows to cards — use 1px Ash borders and surface color contrast (Parchment → Periwinkle) for elevation instead</span></li></div><script>$RS("S:5","P:5")</script><div hidden id="S:6"><li class="flex items-start gap-2 text-sm text-foreground"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-x mt-0.5 size-4 shrink-0 text-red-500" aria-hidden="true"><path d="M18 6 6 18"></path><path d="m6 6 12 12"></path></svg><span>Never use corner radii below 16px on cards or below 100px on buttons — the system is pill-and-soft-rect, never sharp</span></li></div><script>$RS("S:6","P:6")</script><div hidden id="S:7"><li class="flex items-start gap-2 text-sm text-foreground"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-x mt-0.5 size-4 shrink-0 text-red-500" aria-hidden="true"><path d="M18 6 6 18"></path><path d="m6 6 12 12"></path></svg><span>Never introduce additional accent colors for UI elements — the pastel palette (Sky, Mint, Coral, Gold) is decorative-only and belongs in illustrations and gradient washes</span></li></div><script>$RS("S:7","P:7")</script><script>$RC("B:1","S:1")</script><script>self.__next_f.push([1,"3a:I[55925,[\"/_next/static/chunks/0mrygax_2m132.js?dpl=dpl_BdwYag37Coka3wCmVQYgfikUc21G\",\"/_next/static/chunks/0d3shmwh5_nmn.js?dpl=dpl_BdwYag37Coka3wCmVQYgfikUc21G\",\"/_next/static/chunks/0w9zxh-w3z4bi.js?dpl=dpl_BdwYag37Coka3wCmVQYgfikUc21G\",\"/_next/static/chunks/023b0pevwkepq.js?dpl=dpl_BdwYag37Coka3wCmVQYgfikUc21G\",\"/_next/static/chunks/11ktc8fnxphx8.js?dpl=dpl_BdwYag37Coka3wCmVQYgfikUc21G\",\"/_next/static/chunks/04eq_ut3lda3~.js?dpl=dpl_BdwYag37Coka3wCmVQYgfikUc21G\",\"/_next/static/chunks/0.jffwitghhk6.js?dpl=dpl_BdwYag37Coka3wCmVQYgfikUc21G\",\"/_next/static/chunks/0b5wrdfrwab.k.js?dpl=dpl_BdwYag37Coka3wCmVQYgfikUc21G\",\"/_next/static/chunks/0i82lysj2jiv0.js?dpl=dpl_BdwYag37Coka3wCmVQYgfikUc21G\"],\"StyleCard\"]\n"])</script><script>self.__next_f.push([1,"37:[\"$\",\"section\",null,{\"className\":\"space-y-6\",\"children\":[[\"$\",\"h2\",null,{\"className\":\"font-heading text-xl font-semibold tracking-heading\",\"children\":\"More like this\"}],[\"$\",\"div\",null,{\"className\":\"grid gap-x-4 gap-y-6 grid-cols-1 sm:grid-cols-2\",\"children\":[[\"$\",\"$L3a\",\"f99aca3e-5289-4595-a7cc-77a72052f4b8\",{\"style\":{\"id\":\"f99aca3e-5289-4595-a7cc-77a72052f4b8\",\"url\":\"https://ventriloc.ca/en\",\"siteName\":\"Ventriloc\",\"screenshotUrl\":\"https://images.refero.design/styles/refero.design/image/476abb55-bbb0-401b-aaa8-ae84a8c6599d.jpg\",\"thumbnailUrl\":\"https://images.refero.design/styles/refero.design/image/ce55babf-08af-4559-854e-772b9fe79253.jpg\",\"iconUrl\":\"https://images.refero.design/styles/refero.design/image/6038e015-c231-4e82-8534-897560584d1f.png\",\"previewVideoUrl\":\"https://images.refero.design/styles/refero.design/video/892d30ae-09fd-4caf-b286-816ab2910a77.mp4\",\"previewVideoPosterUrl\":\"https://images.refero.design/styles/refero.design/image/b67fcb00-4cc2-4e53-85c1-7e91cbd26a46.jpg\",\"previewVideoWidth\":1200,\"previewVideoHeight\":750,\"previewVideoDetailUrl\":\"https://images.refero.design/styles/refero.design/video/ccf1c2b5-706d-43bd-b949-920f451bb947.mp4\",\"previewVideoDetailPosterUrl\":\"https://images.refero.design/styles/refero.design/image/aca51ee9-42c5-44ac-b384-5e0c69d4c3d5.jpg\",\"previewVideoDetailWidth\":1600,\"previewVideoDetailHeight\":1000,\"previewVideoDurationMs\":6567,\"colorScheme\":\"light\",\"colors\":[{\"name\":\"Graphite\",\"hex\":\"#202020\",\"gradient\":\"$undefined\"},{\"name\":\"Canvas White\",\"hex\":\"#ffffff\",\"gradient\":\"$undefined\"},{\"name\":\"Ash\",\"hex\":\"#efefef\",\"gradient\":\"$undefined\"},{\"name\":\"Fog\",\"hex\":\"#f5f5f5\",\"gradient\":\"$undefined\"},{\"name\":\"Ivory\",\"hex\":\"#ebe6dd\",\"gradient\":\"$undefined\"},{\"name\":\"Steel\",\"hex\":\"#4d4d4d\",\"gradient\":\"$undefined\"}],\"fonts\":[\"PolySans\",\"Inter\"],\"northStar\":\"Editorial data observatory on warm paper — a single orange ember punctuating monochrome precision.\",\"managementSignals\":[],\"createdAt\":\"2026-05-07 02:11:42.689953\"},\"compact\":true}],[\"$\",\"$L3a\",\"8401cb26-91a3-4b46-941e-1c75790821eb\",{\"style\":{\"id\":\"8401cb26-91a3-4b46-941e-1c75790821eb\",\"url\":\"https://www.monologue.to\",\"siteName\":\"Monologue\",\"screenshotUrl\":\"https://images.refero.design/styles/refero.design/image/fde00015-3042-4860-a7a8-a584abf367f4.jpg\",\"thumbnailUrl\":\"https://images.refero.design/styles/refero.design/image/d596e00f-4bcf-4c3a-b9c5-ca1c818e7d12.jpg\",\"iconUrl\":null,\"previewVideoUrl\":\"https://images.refero.design/styles/refero.design/video/3e0491a5-0715-47fd-ae82-c40a9376bce9.mp4\",\"previewVideoPosterUrl\":\"https://images.refero.design/styles/refero.design/image/cfa9af99-c1c8-493a-9ed5-c1bf50d9c8ce.jpg\",\"previewVideoWidth\":1200,\"previewVideoHeight\":750,\"previewVideoDetailUrl\":\"https://images.refero.design/styles/refero.design/video/3bee4218-8fe3-4ae7-a209-b808015be98c.mp4\",\"previewVideoDetailPosterUrl\":\"https://images.refero.design/styles/refero.design/image/9238a9ae-a716-40a5-aca0-ae70f2f65e70.jpg\",\"previewVideoDetailWidth\":1600,\"previewVideoDetailHeight\":1000,\"previewVideoDurationMs\":30520,\"colorScheme\":\"dark\",\"colors\":[{\"name\":\"Electric Cyan\",\"hex\":\"#19d0e8\",\"gradient\":\"$undefined\"},{\"name\":\"Sky Signal\",\"hex\":\"#44ccff\",\"gradient\":\"$undefined\"},{\"name\":\"Deep Teal\",\"hex\":\"#062f34\",\"gradient\":\"$undefined\"},{\"name\":\"Void Black\",\"hex\":\"#000000\",\"gradient\":\"$undefined\"},{\"name\":\"Obsidian\",\"hex\":\"#010101\",\"gradient\":\"$undefined\"},{\"name\":\"Midnight Surface\",\"hex\":\"#191919\",\"gradient\":\"$undefined\"}],\"fonts\":[\"sans-serif\",\"Instrument Serif\",\"DM Mono\",\"Geist\",\"system-ui\",\"SF Pro Display Regular\"],\"northStar\":\"Velvet library with a single blue spark. A vast dark room where a single italic serif headline commands attention and one cyan glow signals action.\",\"managementSignals\":[],\"createdAt\":\"2026-04-30 00:19:04.972736\"},\"compact\":true}],[\"$\",\"$L3a\",\"3f2b79c1-d980-4380-a903-29856975fc37\",{\"style\":{\"id\":\"3f2b79c1-d980-4380-a903-29856975fc37\",\"url\":\"https://midday.ai\",\"siteName\":\"Midday\",\"screenshotUrl\":\"https://images.refero.design/styles/refero.design/image/5e426d8f-9d2c-4586-9b9d-29cbbff76648.jpg\",\"thumbnailUrl\":\"https://images.refero.design/styles/refero.design/image/a33c7b65-1bfc-4926-9c7a-5d0661894c90.jpg\",\"iconUrl\":null,\"previewVideoUrl\":\"https://images.refero.design/styles/refero.design/video/1333f37f-5032-4660-9fa5-d91ec9e1dba3.mp4\",\"previewVideoPosterUrl\":\"https://images.refero.design/styles/refero.design/image/324811a1-7d7b-4d6c-bd54-3f11e65e20bf.jpg\",\"previewVideoWidth\":1200,\"previewVideoHeight\":750,\"previewVideoDetailUrl\":\"https://images.refero.design/styles/refero.design/video/bbebffbe-8c27-4ced-bae3-b15f2dd4fe76.mp4\",\"previewVideoDetailPosterUrl\":\"https://images.refero.design/styles/refero.design/image/0ba618c2-8bbc-4e08-ba60-180bd4484a1e.jpg\",\"previewVideoDetailWidth\":1600,\"previewVideoDetailHeight\":1000,\"previewVideoDurationMs\":11640,\"colorScheme\":\"light\",\"colors\":[{\"name\":\"Parchment\",\"hex\":\"#dbdad7\",\"gradient\":\"$undefined\"},{\"name\":\"Paper\",\"hex\":\"#ffffff\",\"gradient\":\"$undefined\"},{\"name\":\"Sand\",\"hex\":\"#e6e4e0\",\"gradient\":\"$undefined\"},{\"name\":\"Ink\",\"hex\":\"#121212\",\"gradient\":\"$undefined\"},{\"name\":\"Smoke\",\"hex\":\"#616161\",\"gradient\":\"$undefined\"},{\"name\":\"Charcoal\",\"hex\":\"#18181b\",\"gradient\":\"$undefined\"}],\"fonts\":[\"Hedvig Letters Sans\",\"Hedvig Letters Serif\"],\"northStar\":\"Editorial broadsheet on parchment — a 72px serif headline over warm stone, spaced sans-serif body text, pill-shaped controls, zero shadows.\",\"managementSignals\":[],\"createdAt\":\"2026-04-30 00:04:36.281551\"},\"compact\":true}],\"$L3b\",\"$L3c\",\"$L3d\",\"$L3e\",\"$L3f\",\"$L40\",\"$L41\",\"$L42\",\"$L43\",\"$L44\",\"$L45\",\"$L46\",\"$L47\",\"$L48\",\"$L49\",\"$L4a\",\"$L4b\"]}]]}]\n"])</script><script>self.__next_f.push([1,"3b:[\"$\",\"$L3a\",\"3b83dfe4-2f53-4a4d-819d-e6045ca5f7dc\",{\"style\":{\"id\":\"3b83dfe4-2f53-4a4d-819d-e6045ca5f7dc\",\"url\":\"https://x.ai\",\"siteName\":\"xAI\",\"screenshotUrl\":\"https://images.refero.design/styles/refero.design/image/65679a4f-527d-4699-86d8-54a47239f221.jpg\",\"thumbnailUrl\":\"https://images.refero.design/styles/refero.design/image/6281684e-704e-4af3-a449-17fc3834023e.jpg\",\"iconUrl\":null,\"previewVideoUrl\":\"https://images.refero.design/styles/refero.design/video/246289f5-bd2a-4dd5-a1b4-7a3de9b652d5.mp4\",\"previewVideoPosterUrl\":\"https://images.refero.design/styles/refero.design/image/b6ce14bb-4899-4482-8b59-e342c1c35e0b.jpg\",\"previewVideoWidth\":1200,\"previewVideoHeight\":750,\"previewVideoDetailUrl\":\"https://images.refero.design/styles/refero.design/video/0b02b4eb-b48e-457c-837a-8818ef4f2efb.mp4\",\"previewVideoDetailPosterUrl\":\"https://images.refero.design/styles/refero.design/image/a55953ac-b3cb-476c-bff4-199403160bae.jpg\",\"previewVideoDetailWidth\":1600,\"previewVideoDetailHeight\":1000,\"previewVideoDurationMs\":13484,\"colorScheme\":\"light\",\"colors\":[{\"name\":\"Jet Ink\",\"hex\":\"#0a0a0a\",\"gradient\":\"$undefined\"},{\"name\":\"Charcoal\",\"hex\":\"#151515\",\"gradient\":\"$undefined\"},{\"name\":\"Fog\",\"hex\":\"#858585\",\"gradient\":\"$undefined\"},{\"name\":\"Pewter\",\"hex\":\"#9d9d9d\",\"gradient\":\"$undefined\"},{\"name\":\"Steel\",\"hex\":\"#545454\",\"gradient\":\"$undefined\"},{\"name\":\"Dove\",\"hex\":\"#d5d9e2\",\"gradient\":\"$undefined\"}],\"fonts\":[\"universalSans\",\"universalSansDisplay\",\"GeistMono\"],\"northStar\":\"warm cream laboratory with a black pill\",\"managementSignals\":[],\"createdAt\":\"2026-01-25 19:14:43\"},\"compact\":true}]\n"])</script><script>self.__next_f.push([1,"3c:[\"$\",\"$L3a\",\"312423bf-72ea-42fb-b8f5-ab0104e778f3\",{\"style\":{\"id\":\"312423bf-72ea-42fb-b8f5-ab0104e778f3\",\"url\":\"https://www.adaline.ai\",\"siteName\":\"Adaline\",\"screenshotUrl\":\"https://images.refero.design/styles/refero.design/image/329632f2-1a3c-462f-ae1d-59b33bb36eb1.jpg\",\"thumbnailUrl\":\"https://images.refero.design/styles/refero.design/image/41f32951-d1a6-4602-8992-1d08c2e8d319.jpg\",\"iconUrl\":null,\"previewVideoUrl\":\"https://images.refero.design/styles/refero.design/video/45f38f30-c043-4fd9-80bd-69d98606b1a7.mp4\",\"previewVideoPosterUrl\":\"https://images.refero.design/styles/refero.design/image/b03016d4-fe35-4412-9cb8-74927c64386d.jpg\",\"previewVideoWidth\":1200,\"previewVideoHeight\":750,\"previewVideoDetailUrl\":\"https://images.refero.design/styles/refero.design/video/5baaa93c-43b4-405c-b26d-7928f5e0be19.mp4\",\"previewVideoDetailPosterUrl\":\"https://images.refero.design/styles/refero.design/image/e3b2cbcf-7130-4c23-ae4a-c6da64d8c277.jpg\",\"previewVideoDetailWidth\":1600,\"previewVideoDetailHeight\":1000,\"previewVideoDurationMs\":35367,\"colorScheme\":\"light\",\"colors\":[{\"name\":\"Forest Ink\",\"hex\":\"#0a1d08\",\"gradient\":\"$undefined\"},{\"name\":\"Olive Press\",\"hex\":\"#2b390a\",\"gradient\":\"$undefined\"},{\"name\":\"Sage Leaf\",\"hex\":\"#4a6d47\",\"gradient\":\"$undefined\"},{\"name\":\"Deep Teal\",\"hex\":\"#2b6b5e\",\"gradient\":\"$undefined\"},{\"name\":\"Crimson Specimen\",\"hex\":\"#991e4b\",\"gradient\":\"$undefined\"},{\"name\":\"Amber Pin\",\"hex\":\"#80581c\",\"gradient\":\"$undefined\"}],\"fonts\":[\"akkurat\",\"Newsreader\",\"Fragment Mono\",\"ui-monospace\",\"GT America Mono\",\"fragmentMono\"],\"northStar\":\"botanist's specimen journal beside a developer's terminal — warm linen pages, sage ink annotations, and tracked mono tags.\",\"managementSignals\":[],\"createdAt\":\"2026-04-30 00:36:11.612039\"},\"compact\":true}]\n"])</script><script>self.__next_f.push([1,"3d:[\"$\",\"$L3a\",\"e0ad1a25-5609-45e6-a355-9bdeec86c5ae\",{\"style\":{\"id\":\"e0ad1a25-5609-45e6-a355-9bdeec86c5ae\",\"url\":\"https://www.coda.co\",\"siteName\":\"Coda\",\"screenshotUrl\":\"https://images.refero.design/styles/refero.design/image/20140c33-8ebb-41e4-88a4-ff797a702b93.jpg\",\"thumbnailUrl\":\"https://images.refero.design/styles/refero.design/image/412495d2-8370-4a74-8bc8-70d368b2b050.jpg\",\"iconUrl\":null,\"previewVideoUrl\":null,\"previewVideoPosterUrl\":null,\"previewVideoWidth\":null,\"previewVideoHeight\":null,\"previewVideoDetailUrl\":null,\"previewVideoDetailPosterUrl\":null,\"previewVideoDetailWidth\":null,\"previewVideoDetailHeight\":null,\"previewVideoDurationMs\":null,\"colorScheme\":\"light\",\"colors\":[{\"name\":\"Cream Parchment\",\"hex\":\"#f8f9eb\",\"gradient\":\"$undefined\"},{\"name\":\"Pure White\",\"hex\":\"#ffffff\",\"gradient\":\"$undefined\"},{\"name\":\"Obsidian\",\"hex\":\"#000000\",\"gradient\":\"$undefined\"},{\"name\":\"Charcoal\",\"hex\":\"#202020\",\"gradient\":\"$undefined\"},{\"name\":\"Sage Mist\",\"hex\":\"#c0c2a9\",\"gradient\":\"$undefined\"},{\"name\":\"Olive Slate\",\"hex\":\"#5a5a4f\",\"gradient\":\"$undefined\"}],\"fonts\":[\"ui-sans-serif\",\"Monument Grotesk (custom)\",\"JetBrains Mono\",\"System UI Sans\"],\"northStar\":\"Monumental letters on warm cream parchment — Coda reads like a hand-set marketplace poster, not a SaaS dashboard.\",\"managementSignals\":[],\"createdAt\":\"2026-04-30 00:41:53.682316\"},\"compact\":true}]\n"])</script><script>self.__next_f.push([1,"3e:[\"$\",\"$L3a\",\"2db41cd9-c898-4f59-b704-3042c0d87f45\",{\"style\":{\"id\":\"2db41cd9-c898-4f59-b704-3042c0d87f45\",\"url\":\"https://www.dittowords.com\",\"siteName\":\"Ditto\",\"screenshotUrl\":\"https://images.refero.design/styles/refero.design/image/3e2c4051-7142-4880-99e3-6ca2e5ccb2a6.jpg\",\"thumbnailUrl\":\"https://images.refero.design/styles/refero.design/image/97b76e99-ac6e-4458-acc0-7a20d8be9802.jpg\",\"iconUrl\":null,\"previewVideoUrl\":\"https://images.refero.design/styles/refero.design/video/9bc7b942-7fc8-4e75-aa26-30da41c115a0.mp4\",\"previewVideoPosterUrl\":\"https://images.refero.design/styles/refero.design/image/66499053-ddb6-48c2-901b-8d6db6397147.jpg\",\"previewVideoWidth\":1200,\"previewVideoHeight\":750,\"previewVideoDetailUrl\":\"https://images.refero.design/styles/refero.design/video/7a16c35f-0ab8-4e09-8d6d-0a194b959d4a.mp4\",\"previewVideoDetailPosterUrl\":\"https://images.refero.design/styles/refero.design/image/4b147390-0577-4af9-9419-0b1e3f49b11f.jpg\",\"previewVideoDetailWidth\":1600,\"previewVideoDetailHeight\":1000,\"previewVideoDurationMs\":19534,\"colorScheme\":\"light\",\"colors\":[{\"name\":\"Parchment\",\"hex\":\"#f7f5f3\",\"gradient\":\"$undefined\"},{\"name\":\"India Ink\",\"hex\":\"#000000\",\"gradient\":\"$undefined\"},{\"name\":\"Charcoal Warm\",\"hex\":\"#222222\",\"gradient\":\"$undefined\"},{\"name\":\"Graphite Warm\",\"hex\":\"#6a6559\",\"gradient\":\"$undefined\"},{\"name\":\"Bone White\",\"hex\":\"#ffffff\",\"gradient\":\"$undefined\"},{\"name\":\"Smoke\",\"hex\":\"#e2e2e2\",\"gradient\":\"$undefined\"}],\"fonts\":[\"ABC Social\",\"ABC Social Extended\",\"ABC Social Condensed\"],\"northStar\":\"marked-up manuscript on warm parchment\",\"managementSignals\":[],\"createdAt\":\"2026-04-30 00:15:35.209705\"},\"compact\":true}]\n"])</script><script>self.__next_f.push([1,"3f:[\"$\",\"$L3a\",\"694723e9-0df7-4b9f-ba07-83fc598532d6\",{\"style\":{\"id\":\"694723e9-0df7-4b9f-ba07-83fc598532d6\",\"url\":\"https://symbolic.ai\",\"siteName\":\"Symbolic.ai\",\"screenshotUrl\":\"https://images.refero.design/styles/refero.design/image/39a13a10-1ae4-4818-99a1-188eb6167311.jpg\",\"thumbnailUrl\":\"https://images.refero.design/styles/refero.design/image/6c5cf797-34de-4fc0-9ca1-880726936552.jpg\",\"iconUrl\":null,\"previewVideoUrl\":\"https://images.refero.design/styles/refero.design/video/c10ad7f6-77dc-423f-9784-e5082059421a.mp4\",\"previewVideoPosterUrl\":\"https://images.refero.design/styles/refero.design/image/809f7206-5f19-4aa1-b789-7f39319bd8c3.jpg\",\"previewVideoWidth\":1200,\"previewVideoHeight\":750,\"previewVideoDetailUrl\":\"https://images.refero.design/styles/refero.design/video/9f038f89-9a14-4b89-bfc8-f90171001369.mp4\",\"previewVideoDetailPosterUrl\":\"https://images.refero.design/styles/refero.design/image/6c314cbe-fc44-4fea-8fe7-467e7f72df8d.jpg\",\"previewVideoDetailWidth\":1600,\"previewVideoDetailHeight\":1000,\"previewVideoDurationMs\":19217,\"colorScheme\":\"light\",\"colors\":[{\"name\":\"Canvas Cream\",\"hex\":\"#fdfcf5\",\"gradient\":\"$undefined\"},{\"name\":\"Ink Black\",\"hex\":\"#000000\",\"gradient\":\"$undefined\"},{\"name\":\"Paper White\",\"hex\":\"#ffffff\",\"gradient\":\"$undefined\"},{\"name\":\"Charcoal\",\"hex\":\"#4c4c4a\",\"gradient\":\"$undefined\"},{\"name\":\"Slate Black\",\"hex\":\"#333231\",\"gradient\":\"$undefined\"},{\"name\":\"Warm Gray\",\"hex\":\"#7f7e7b\",\"gradient\":\"$undefined\"}],\"fonts\":[\"sans-serif\",\"Suisse Works\",\"Open Runde\",\"Geist Mono\",\"Grenze Gotisch\",\"Inter\"],\"northStar\":\"editorial newsroom on cream paper. A broadsheet masthead in serif type, floating on warm off-white stock, with soft tan shadows that make every card feel like it was set in letterpress — not rendered.\",\"managementSignals\":[],\"createdAt\":\"2026-04-30 00:18:51.694924\"},\"compact\":true}]\n"])</script><script>self.__next_f.push([1,"40:[\"$\",\"$L3a\",\"34d438ad-0647-471e-9a6f-7c1fa29d5df6\",{\"style\":{\"id\":\"34d438ad-0647-471e-9a6f-7c1fa29d5df6\",\"url\":\"https://www.browserbase.com\",\"siteName\":\"Browserbase\",\"screenshotUrl\":\"https://images.refero.design/styles/refero.design/image/68ba137b-d107-428e-9ba5-0d0798c3bdcb.jpg\",\"thumbnailUrl\":\"https://images.refero.design/styles/refero.design/image/eabc20a9-305c-4df3-8860-116a18dbef19.jpg\",\"iconUrl\":\"https://images.refero.design/styles/refero.design/image/c6320b30-c3a1-400c-8f9a-75ee2f357dcb.png\",\"previewVideoUrl\":\"https://images.refero.design/styles/refero.design/video/2c4c7d8d-e15a-4239-9efb-c9b7c33db3f2.mp4\",\"previewVideoPosterUrl\":\"https://images.refero.design/styles/refero.design/image/37f2e47d-da68-46e3-a2a2-d673cf3eb0f3.jpg\",\"previewVideoWidth\":1200,\"previewVideoHeight\":750,\"previewVideoDetailUrl\":\"https://images.refero.design/styles/refero.design/video/90452938-24bf-4521-85c5-6a8451173ef3.mp4\",\"previewVideoDetailPosterUrl\":\"https://images.refero.design/styles/refero.design/image/64c8ba6a-17ec-44f4-aae1-c0a5a8082ae6.jpg\",\"previewVideoDetailWidth\":1600,\"previewVideoDetailHeight\":1000,\"previewVideoDurationMs\":18667,\"colorScheme\":\"light\",\"colors\":[{\"name\":\"Ink Black\",\"hex\":\"#000000\",\"gradient\":\"$undefined\"},{\"name\":\"Paper White\",\"hex\":\"#ffffff\",\"gradient\":\"$undefined\"},{\"name\":\"Faint Slate\",\"hex\":\"#f8fafc\",\"gradient\":\"$undefined\"},{\"name\":\"Lavender Mist\",\"hex\":\"#e2e9f3\",\"gradient\":\"$undefined\"},{\"name\":\"Blue-Gray Mist\",\"hex\":\"#c5d3e8\",\"gradient\":\"$undefined\"},{\"name\":\"Cream Wash\",\"hex\":\"#fffde6\",\"gradient\":\"$undefined\"}],\"fonts\":[\"plain\",\"gtPlanar\",\"gtStandardMono\"],\"northStar\":\"editorial broadsheet meets data terminal — a single hot orange punctuating a near-monochrome field of oversized GT Planar headlines, soft pastel card surfaces, and tiny mono metadata.\",\"managementSignals\":[],\"createdAt\":\"2026-05-07 18:36:19.451902\"},\"compact\":true}]\n"])</script><script>self.__next_f.push([1,"41:[\"$\",\"$L3a\",\"c90e63f8-76c1-4159-9460-29e0d18751ae\",{\"style\":{\"id\":\"c90e63f8-76c1-4159-9460-29e0d18751ae\",\"url\":\"https://www.parloa.com\",\"siteName\":\"Parloa\",\"screenshotUrl\":\"https://images.refero.design/styles/refero.design/image/266657b1-3db6-4b26-a9d7-34bfeea53f57.jpg\",\"thumbnailUrl\":\"https://images.refero.design/styles/refero.design/image/a52d25ad-1ad0-4261-b8ef-0ab71af9466e.jpg\",\"iconUrl\":\"https://images.refero.design/styles/refero.design/image/96958f3f-acaa-45f3-8fab-e25394b7485b.png\",\"previewVideoUrl\":\"https://images.refero.design/styles/refero.design/video/d8fc93fb-a4e8-41e7-8dd8-b2cb18443f77.mp4\",\"previewVideoPosterUrl\":\"https://images.refero.design/styles/refero.design/image/85432b60-d146-4249-80d5-9542b3ef6fb8.jpg\",\"previewVideoWidth\":1200,\"previewVideoHeight\":750,\"previewVideoDetailUrl\":\"https://images.refero.design/styles/refero.design/video/99b3767a-a29a-4a8c-8a62-1909ccc6ce56.mp4\",\"previewVideoDetailPosterUrl\":\"https://images.refero.design/styles/refero.design/image/bcd3dcfa-66a5-44f2-8cbb-adfb1766494a.jpg\",\"previewVideoDetailWidth\":1600,\"previewVideoDetailHeight\":1000,\"previewVideoDurationMs\":18284,\"colorScheme\":\"light\",\"colors\":[{\"name\":\"Ink Black\",\"hex\":\"#1f1c1b\",\"gradient\":\"$undefined\"},{\"name\":\"Paper White\",\"hex\":\"#ffffff\",\"gradient\":\"$undefined\"},{\"name\":\"Canvas Cream\",\"hex\":\"#ebe9e1\",\"gradient\":\"$undefined\"},{\"name\":\"Linen\",\"hex\":\"#f5f4f0\",\"gradient\":\"$undefined\"},{\"name\":\"Stone\",\"hex\":\"#a69b92\",\"gradient\":\"$undefined\"},{\"name\":\"Hairline\",\"hex\":\"#d9d6ce\",\"gradient\":\"$undefined\"}],\"fonts\":[\"Exposure30\",\"Geist\"],\"northStar\":\"warm editorial paper with ink and highlighter\",\"managementSignals\":[],\"createdAt\":\"2026-05-10 22:04:08.161187\"},\"compact\":true}]\n"])</script><script>self.__next_f.push([1,"42:[\"$\",\"$L3a\",\"8b5cfe6d-a2bd-4edb-854e-9185cec46c09\",{\"style\":{\"id\":\"8b5cfe6d-a2bd-4edb-854e-9185cec46c09\",\"url\":\"https://panxo.com\",\"siteName\":\"Panxo\",\"screenshotUrl\":\"https://images.refero.design/styles/refero.design/image/24cf39f9-9f6b-47e0-bf8c-0cea968c8810.jpg\",\"thumbnailUrl\":\"https://images.refero.design/styles/refero.design/image/3a25a83a-83f7-4c8e-9a5c-02698e06bdaa.jpg\",\"iconUrl\":null,\"previewVideoUrl\":\"https://images.refero.design/styles/refero.design/video/975500e2-5f12-4e31-bb64-a98063b03e92.mp4\",\"previewVideoPosterUrl\":\"https://images.refero.design/styles/refero.design/image/51bbf32c-9f6b-415e-9143-381bb8c7fd47.jpg\",\"previewVideoWidth\":1200,\"previewVideoHeight\":750,\"previewVideoDetailUrl\":\"https://images.refero.design/styles/refero.design/video/fb771e93-947c-4800-97ea-738c6e9b7397.mp4\",\"previewVideoDetailPosterUrl\":\"https://images.refero.design/styles/refero.design/image/1e700666-da05-4e56-8a18-2f53f1c5d38f.jpg\",\"previewVideoDetailWidth\":1600,\"previewVideoDetailHeight\":1000,\"previewVideoDurationMs\":27360,\"colorScheme\":\"light\",\"colors\":[{\"name\":\"Coal Ink\",\"hex\":\"#1c1a17\",\"gradient\":\"$undefined\"},{\"name\":\"Ledger White\",\"hex\":\"#fafafa\",\"gradient\":\"$undefined\"},{\"name\":\"Parchment\",\"hex\":\"#f7f3eb\",\"gradient\":\"$undefined\"},{\"name\":\"Ash\",\"hex\":\"#f1f1f1\",\"gradient\":\"$undefined\"},{\"name\":\"Slate Mid\",\"hex\":\"#7e7d7b\",\"gradient\":\"$undefined\"},{\"name\":\"Graphite\",\"hex\":\"#5a5957\",\"gradient\":\"$undefined\"}],\"fonts\":[\"Mona Sans\",\"Inter\",\"sans-serif\"],\"northStar\":\"Data terminal in warm ink — every surface echoes ledger paper, every accent reads like a highlighted cell.\",\"managementSignals\":[],\"createdAt\":\"2026-03-30 09:16:57\"},\"compact\":true}]\n"])</script><script>self.__next_f.push([1,"43:[\"$\",\"$L3a\",\"4d832c12-dd14-45b0-bba7-2d3bc25d8264\",{\"style\":{\"id\":\"4d832c12-dd14-45b0-bba7-2d3bc25d8264\",\"url\":\"https://loops.so\",\"siteName\":\"Loops\",\"screenshotUrl\":\"https://images.refero.design/styles/refero.design/image/71871994-7a1d-45aa-a6a3-fc9ba73ccffb.jpg\",\"thumbnailUrl\":\"https://images.refero.design/styles/refero.design/image/562b2822-753a-4d97-95b3-c41edeaeeaf1.jpg\",\"iconUrl\":null,\"previewVideoUrl\":null,\"previewVideoPosterUrl\":null,\"previewVideoWidth\":null,\"previewVideoHeight\":null,\"previewVideoDetailUrl\":null,\"previewVideoDetailPosterUrl\":null,\"previewVideoDetailWidth\":null,\"previewVideoDetailHeight\":null,\"previewVideoDurationMs\":null,\"colorScheme\":\"light\",\"colors\":[{\"name\":\"Parchment\",\"hex\":\"#faf9f7\",\"gradient\":\"$undefined\"},{\"name\":\"Paper\",\"hex\":\"#ffffff\",\"gradient\":\"$undefined\"},{\"name\":\"Mist\",\"hex\":\"#f1efef\",\"gradient\":\"$undefined\"},{\"name\":\"Stone-200\",\"hex\":\"#e7e5e4\",\"gradient\":\"$undefined\"},{\"name\":\"Stone-300\",\"hex\":\"#d6d3d1\",\"gradient\":\"$undefined\"},{\"name\":\"Stone-400\",\"hex\":\"#a8a29e\",\"gradient\":\"$undefined\"}],\"fonts\":[\"sans-serif\",\"Newsreader\",\"Inter\",\"ui-monospace\",\"ui-sans-serif\",\"Iowan Old Style\"],\"northStar\":\"Warm parchment behind a serif headline — like a stationer's print proof lit by afternoon sun.\",\"managementSignals\":[],\"createdAt\":\"2026-04-30 00:50:23.096135\"},\"compact\":true}]\n"])</script><script>self.__next_f.push([1,"44:[\"$\",\"$L3a\",\"c809190a-035c-458d-87ed-4758807dd84e\",{\"style\":{\"id\":\"c809190a-035c-458d-87ed-4758807dd84e\",\"url\":\"https://axiom.co\",\"siteName\":\"Axiom\",\"screenshotUrl\":\"https://images.refero.design/styles/refero.design/image/1b5c27c9-e0be-475f-a9be-70850759dd8a.jpg\",\"thumbnailUrl\":\"https://images.refero.design/styles/refero.design/image/5f307483-b9fc-4765-a81c-ee710ceaa4d6.jpg\",\"iconUrl\":null,\"previewVideoUrl\":\"https://images.refero.design/styles/refero.design/video/6f530b45-fda0-4855-b78c-4558f35bedbf.mp4\",\"previewVideoPosterUrl\":\"https://images.refero.design/styles/refero.design/image/3ce49ef3-22c9-48de-adcb-c765fe292c3c.jpg\",\"previewVideoWidth\":1200,\"previewVideoHeight\":750,\"previewVideoDetailUrl\":\"https://images.refero.design/styles/refero.design/video/ee044163-bfd1-473f-8443-ae963b5c85ad.mp4\",\"previewVideoDetailPosterUrl\":\"https://images.refero.design/styles/refero.design/image/4035444e-8fff-4aef-8f3b-2a7f780e70a8.jpg\",\"previewVideoDetailWidth\":1600,\"previewVideoDetailHeight\":1000,\"previewVideoDurationMs\":23480,\"colorScheme\":\"dark\",\"colors\":[{\"name\":\"Void\",\"hex\":\"#000000\",\"gradient\":\"$undefined\"},{\"name\":\"Carbon\",\"hex\":\"#111111\",\"gradient\":\"$undefined\"},{\"name\":\"Graphite\",\"hex\":\"#191919\",\"gradient\":\"$undefined\"},{\"name\":\"Iron\",\"hex\":\"#202020\",\"gradient\":\"$undefined\"},{\"name\":\"Slate\",\"hex\":\"#3a3a3a\",\"gradient\":\"$undefined\"},{\"name\":\"Pewter\",\"hex\":\"#505050\",\"gradient\":\"$undefined\"}],\"fonts\":[\"BerkeleyMono\",\"Inter\"],\"northStar\":\"Terminal window at midnight — flat black canvas, monospaced text, and one orange cursor blinking\",\"management