# Getharvest — Style Reference
> Golden hour workbench — warm cream canvas, white floating cards, and one vivid orange flame.

**Theme:** light

Harvest uses a sunlit productivity-workspace language: warm cream canvas (#fff8f1) replaces the typical SaaS white, giving every screen a golden-hour warmth, while white cards and panels float above that base for product surfaces. One vivid orange (#fa5d00) carries all the energy — every CTA, link, icon accent, and brand border — making it the only chromatic decision in an otherwise achromatic system of warm grays. Typography is confident and editorial: a geometric sans (MuotoWeb) for everything functional, with a serif display face (Monarch) reserved for hero-grade emotional moments. Components are soft and tactile: 16–20px radii, low warm-tinted shadows, generous breathing room, and decorative orange wash gradients that suggest movement without ever competing with content.

## Tokens — Colors

| Name | Value | Token | Role |
|------|-------|-------|------|
| Harvest Flame | `#fa5d00` | `--color-harvest-flame` | Primary CTA fill, active nav indicator, brand link color, heading underlines — warm vermilion that reads as energetic but not aggressive, the single chromatic decision in an otherwise achromatic system |
| Marigold Glow | `#fee3b5` | `--color-marigold-glow` | Soft warm highlight wash on cards, decorative glow tint behind product UI — never functional, only atmospheric |
| Parchment Shadow | `#e3d6c5` | `--color-parchment-shadow` | Warm-tinted card shadow color, subtle image shadow — the shadow hue is not neutral gray but matches the cream base |
| Ink Black | `#1d1e1c` | `--color-ink-black` | Primary text, icon strokes, nav borders, card headings — warm near-black rather than pure #000, preserves the system warmth |
| Paper White | `#ffffff` | `--color-paper-white` | Card surfaces, input fields, elevated panels, button text on orange fill |
| Cream Canvas | `#fff8f1` | `--color-cream-canvas` | Page background, hero section base, nav backdrop — the signature warm cream that replaces standard SaaS white |
| Mist Gray | `#d9d9d9` | `--color-mist-gray` | Hairline dividers, subtle borders on neutral surfaces |
| Warm Stone | `#615f5c` | `--color-warm-stone` | Secondary body text, list items, muted icon strokes |
| Driftwood | `#8e8b87` | `--color-driftwood` | Tertiary body text, decorative strokes, subtle metadata |
| Ironwood | `#4a4a47` | `--color-ironwood` | Strong secondary text, emphasized muted labels |
| Ash | `#777571` | `--color-ash` | Helper text, placeholder-adjacent copy, low-priority borders |
| Bone | `#c0bbb6` | `--color-bone` | Input borders, form field outlines at rest |
| Smoke | `#a5a19c` | `--color-smoke` | Disabled text, decorative borders, very low-priority separators |
| Graphite | `#999999` | `--color-graphite` | List borders, tertiary structural lines |

## Tokens — Typography

### MuotoWeb — Primary UI and body typeface — geometric sans covering navigation, buttons, body copy, subheadings, and most headings up to 50px. Custom-drawn letterforms give it warmth that generic Inter or Helvetica cannot: slightly humanist terminals and open apertures that read friendly rather than cold. · `--font-muotoweb`
- **Substitute:** Inter or Sohne
- **Weights:** 400, 500, 600, 700
- **Sizes:** 13, 14, 16, 17, 18, 20, 22, 24, 25, 26, 28, 34, 48, 50
- **Line height:** 1.15–1.50
- **Letter spacing:** 0.015em
- **OpenType features:** `"ss01" on, "cv11" on`
- **Role:** Primary UI and body typeface — geometric sans covering navigation, buttons, body copy, subheadings, and most headings up to 50px. Custom-drawn letterforms give it warmth that generic Inter or Helvetica cannot: slightly humanist terminals and open apertures that read friendly rather than cold.

### Monarch — Hero display serif — used only for the largest emotional headline (72px) where editorial weight is needed. The serif is the signature contrast against MuotoWeb's sans body: the page whispers functional in sans, then ROARS one moment in serif. Reserve for hero/page-title moments only. · `--font-monarch`
- **Substitute:** GT Super or Tiempos Headline
- **Weights:** 400
- **Sizes:** 72
- **Line height:** 1.20
- **Role:** Hero display serif — used only for the largest emotional headline (72px) where editorial weight is needed. The serif is the signature contrast against MuotoWeb's sans body: the page whispers functional in sans, then ROARS one moment in serif. Reserve for hero/page-title moments only.

### Type Scale

| Role | Size | Line Height | Letter Spacing | Token |
|------|------|-------------|----------------|-------|
| caption | 13px | 1.35 | 0.2px | `--text-caption` |
| subheading | 18px | 1.4 | 0.27px | `--text-subheading` |
| heading-sm | 20px | 1.3 | 0.3px | `--text-heading-sm` |
| heading | 24px | 1.26 | 0.36px | `--text-heading` |
| heading-lg | 28px | 1.2 | 0.42px | `--text-heading-lg` |
| display | 48px | 1.15 | 0.72px | `--text-display` |
| display-lg | 72px | 1.2 | — | `--text-display-lg` |

## Tokens — Spacing & Shapes

**Density:** comfortable

### Spacing Scale

| Name | Value | Token |
|------|-------|-------|
| 4 | 4px | `--spacing-4` |
| 5 | 5px | `--spacing-5` |
| 7 | 7px | `--spacing-7` |
| 10 | 10px | `--spacing-10` |
| 14 | 14px | `--spacing-14` |
| 15 | 15px | `--spacing-15` |
| 16 | 16px | `--spacing-16` |
| 20 | 20px | `--spacing-20` |
| 22 | 22px | `--spacing-22` |
| 25 | 25px | `--spacing-25` |
| 30 | 30px | `--spacing-30` |
| 35 | 35px | `--spacing-35` |
| 40 | 40px | `--spacing-40` |
| 50 | 50px | `--spacing-50` |
| 100 | 100px | `--spacing-100` |
| 113 | 113px | `--spacing-113` |

### Border Radius

| Element | Value |
|---------|-------|
| tags | 999px |
| cards | 20px |
| images | 16px |
| inputs | 16px |
| buttons | 16px |

### Shadows

| Name | Value | Token |
|------|-------|-------|
| sm | `rgba(0, 0, 0, 0.2) 0px 1px 4px 0px` | `--shadow-sm` |
| lg | `rgba(250, 166, 0, 0.25) 6px 4px 24px 0px` | `--shadow-lg` |

### Layout

- **Page max-width:** 1200px
- **Section gap:** 64-80px
- **Card padding:** 32-40px
- **Element gap:** 16-24px

## Components

### Primary CTA Button
**Role:** Filled orange action button — the system’s single most important interactive element

Fill: #fa5d00. Text: #ffffff, MuotoWeb 16px weight 600, letter-spacing 0.015em. Padding: 12px 24px. Border-radius: 16px. Shadow: rgba(0,0,0,0.2) 0px 1px 4px 0px for subtle lift. Hover darkens the orange ~10%. Used for: 'Try Harvest free', 'Get started for free', 'Start your free trial'.

### Ghost/Text Link
**Role:** Secondary action — 'Learn more' style links under feature cards

Text: #fa5d00, MuotoWeb 16px weight 500. No background, no border, no padding. May carry a small → arrow icon. Underline appears on hover.

### Email Input Field
**Role:** Hero form input for email capture

Fill: #ffffff. Border: 1px solid #c0bbb6. Border-radius: 16px. Padding: 14px 20px. Placeholder text: #8e8b87 16px. Focus ring: #fa5d00 2px outline with 4px offset.

### Feature Card
**Role:** Three-column feature highlight card with icon, heading, body, and link

Fill: #fff8f1 (cream, same as canvas — depth comes from shadow not contrast). Border-radius: 20px. Padding: 40px 32px. Optional shadow: rgba(250,166,0,0.25) 6px 4px 24px 0px for warm glow. Icon: dark #1d1e1c at 48px. Heading: MuotoWeb 20-24px weight 600 #1d1e1c. Body: 16px weight 400 #615f5c. Link: orange #fa5d00 weight 500.

### Integration Logo Circle
**Role:** Round badge displaying third-party app logos

48px circle, fill #ffffff, contains colorful third-party brand logo (not a system color — logos are literal brand marks). Arranged in horizontal or grid patterns to show ecosystem breadth.

### Navigation Bar
**Role:** Top sticky navigation with logo, menu items, sign-in, and primary CTA

Background: #fff8f1 with 1px solid #fff8f1 border (subtle). Logo: orange 'harvest' wordmark with bar-chart icon. Nav links: MuotoWeb 16px weight 500 #1d1e1c. Dropdown chevrons on Features, Why Harvest, Resources. Right side: 'Sign in' as ghost link + 'Try Harvest free' as primary orange CTA.

### Dashboard Preview Card
**Role:** Product screenshot container — shows actual app UI as social proof

White surface (#ffffff) with border-radius 16px, soft shadow, contains literal Harvest product screenshots (timesheet grid, profitability report with bar/line charts). Used in hero area as floating proof elements.

### Section Heading (Eyebrow + Title)
**Role:** Reusable section header pattern with small uppercase label and large title

Eyebrow: MuotoWeb 14px weight 600 uppercase, letter-spacing 0.015em, #fa5d00 (e.g., 'WHY HARVEST'). Title: MuotoWeb 34-48px weight 400-500 #1d1e1c, centered, max-width ~700px. Optional subtitle in #615f5c 17px.

### Trust Badge Logo Row
**Role:** Grayscale logo strip for social proof — 'TRUSTED BY 70,000+ COMPANIES'

Label: MuotoWeb 13px weight 600 uppercase #615f5c with #fa5d00 highlight on the number. Logos: rendered in #1d1e1c grayscale at 60-80% opacity, evenly spaced horizontal row. No logos are colored — the grayscale treatment keeps the orange accent uncontested.

### Hero Gradient Wash
**Role:** Decorative flowing gradient background behind hero content

Soft flowing wash of #fa5d00, #fee3b5, and warm peach tones rendered as an organic flowing shape (not a hard gradient strip). Low opacity (~30-50%), positioned behind the product preview cards. Creates sense of warmth and movement without ever competing with text.

### Feature Grid (2-column)
**Role:** Alternating two-column layout: heading+body left, product screenshot right

Max-width container with 2 equal columns, 40px gap. Left column: heading, paragraph body, optional inline CTA. Right column: product screenshot or illustration. Background alternates: #fff8f1 base with white cards floating above.

## Do's and Don'ts

### Do
- Use #fa5d00 exclusively for primary actions, active states, and brand moments — never for body text or large decorative areas where it would overwhelm the cream canvas
- Set all page backgrounds to #fff8f1 (cream), not #ffffff — the warmth is the system identity
- Reserve Monarch serif for hero-grade 72px display headlines only; use MuotoWeb for all headings 50px and below
- Apply 16px radius to all buttons and inputs, 20px radius to all cards — these two values are the system's tactile signature
- Use 0.015em positive letter-spacing on all MuotoWeb text — this tracks-wide feel softens the geometric sans into something friendlier
- Keep shadows warm-tinted (rgba(250,166,0,0.25) for cards, rgba(0,0,0,0.2) for buttons) — never use cold blue or neutral gray shadows that would fight the cream base
- Place trust/partner logos in grayscale (#1d1e1c) so the orange accent remains the only chromatic focal point

### Don't
- Don't use #ffffff as the page background — the cream #fff8f1 canvas IS the brand
- Don't introduce a second accent color — the system's discipline is one orange against warm neutrals
- Don't use Monarch serif for body text, subheadings, or anything under 48px — it dilutes the hero impact
- Don't use sharp 0-4px corner radii on cards or buttons — the 16-20px softness is essential to the warm tactile feel
- Don't use cool blue-tinted shadows or borders — everything in this system carries a warm undertone
- Don't apply saturated colors to large background fills — keep the orange small, concentrated, and functional
- Don't use pure #000000 for text — #1d1e1c (warm near-black) preserves the system's warmth

## Surfaces

| Level | Name | Value | Purpose |
|-------|------|-------|---------|
| 1 | Cream Canvas | `#fff8f1` | Page-level background — the warm cream base that defines the entire system mood |
| 2 | Paper White | `#ffffff` | Card and elevated surface — floats above the cream canvas to create product depth |
| 3 | Orange Brand Surface | `#fa5d00` | CTA buttons, active states, and brand accent surfaces — the only chromatic surface |

## Elevation

- **Primary CTA Button:** `rgba(0, 0, 0, 0.2) 0px 1px 4px 0px`
- **Feature Card (soft warm glow):** `rgba(250, 166, 0, 0.25) 6px 4px 24px 0px`

## Agent Prompt Guide

Quick Color Reference:
- text: #1d1e1c
- background: #fff8f1 (page) / #ffffff (cards)
- border: #c0bbb6 (input) / #d9d9d9 (divider)
- accent: #fa5d00 (links, icons, small highlights)
- primary action: #fa5d00 (filled action)
- secondary text: #615f5c

3 Example Component Prompts:

1. Create a Primary Action Button: #fa5d00 background, #1d1e1c text, 9999px radius, compact pill padding. Use this filled treatment for the main CTA.

2. Create a feature card on cream background (#fff8f1). White or cream fill, 20px border-radius, 40px 32px padding. Dark icon (#1d1e1c) at 48px centered top. Heading: MuotoWeb 22px weight 600 #1d1e1c. Body text: 16px weight 400 #615f5c. Orange 'Learn more' link (#fa5d00, weight 500) with → arrow.


## Visual Language

Imagery: Product UI screenshots are the dominant visual — real Harvest app interfaces (timesheets, profitability charts) shown as floating cards in the hero and section blocks. No stock photography, no lifestyle imagery, no abstract 3D renders. The app UI IS the hero. 

Treatment: Product screenshots are presented in white cards with 16px radius and soft warm-tinted shadows, often floating at slight angles or with offset positions to create depth. The hero features a flowing warm gradient wash (orange to yellow to peach) that sits behind the product cards, suggesting motion and warmth without literal illustration.

Icons: Dark (#1d1e1c), filled or outlined geometric shapes at 48px — stopwatch for time tracking, pie chart for reports, receipt for invoicing. Icons sit centered above feature card headings, no color, no decoration. Integration logos appear in 48px white circles with their literal brand colors (the only place external color enters the system). 

Trust/social proof: Partner logos rendered in grayscale at 60-80% opacity in a single horizontal row under a small uppercase label. The grayscale treatment is deliberate — it prevents partner brand colors from competing with Harvest's orange.

Density: Text-dominant with product screenshots as visual punctuation. The cream canvas and generous spacing (64-80px section gaps) create breathing room. Information density is moderate — comfortable for reading, not packed.

## Layout Patterns

Page model: Centered max-width container (~1200px) with generous horizontal padding. Full-bleed cream background extends edge-to-edge, but content is always centered and constrained.

Hero pattern: Centered headline + subtitle + email capture form over a flowing warm gradient wash with two floating product preview cards (dashboard screenshots) positioned left and right at slight offsets. The hero is editorial in feel — large serif headline, soft warm atmosphere, product proof floating around it.

Section rhythm: Consistent vertical rhythm with 64-80px gaps between sections. Sections alternate between centered text-only blocks and 2-column text+screenshot layouts. No alternating dark/light bands — the entire page lives on the warm cream canvas.

Content arrangement: After the centered hero, content moves into a repeating pattern: centered section heading (eyebrow + title), then either a 3-column feature card grid or 2-column alternating text+image blocks. The 2-column blocks are not strictly alternating — both columns can be filled with product screenshots rather than one text/one image.

Grid usage: 3-column card grid for the 'Why Harvest' feature highlights. 2-column grid for detailed feature breakdowns (simple time tracking, integrations, capacity, budget). 1-column centered stack for the email capture CTA.

Navigation: Sticky top bar with logo left, menu center, sign-in + primary CTA right. No sidebar, no mega-menu visible — dropdown indicators suggest sub-menus on hover but the top bar stays slim and clean.

## Similar Brands

- **Toggl Track** — Same warm cream + orange palette, same time-tracking product focus, same soft rounded card aesthetic with single-accent-color discipline
- **FreshBooks** — Same warm approachable SaaS feel with orange accent, cream backgrounds, and product-screenshot-as-hero treatment
- **Notion** — Same generous whitespace and warm-neutral palette approach, though Notion uses black where Harvest uses warm near-black and orange
- **Basecamp** — Same friendly productivity-tool voice with warm backgrounds and rounded components, though Basecamp leans more colorful where Harvest stays disciplined to one orange
- **QuickBooks** — Same professional-services workflow focus with warm UI palette and product-preview hero pattern

## Quick Start

### CSS Custom Properties

```css
:root {
  /* Colors */
  --color-harvest-flame: #fa5d00;
  --color-marigold-glow: #fee3b5;
  --color-parchment-shadow: #e3d6c5;
  --color-ink-black: #1d1e1c;
  --color-paper-white: #ffffff;
  --color-cream-canvas: #fff8f1;
  --color-mist-gray: #d9d9d9;
  --color-warm-stone: #615f5c;
  --color-driftwood: #8e8b87;
  --color-ironwood: #4a4a47;
  --color-ash: #777571;
  --color-bone: #c0bbb6;
  --color-smoke: #a5a19c;
  --color-graphite: #999999;

  /* Typography — Font Families */
  --font-muotoweb: 'MuotoWeb', ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
  --font-monarch: 'Monarch', ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;

  /* Typography — Scale */
  --text-caption: 13px;
  --leading-caption: 1.35;
  --tracking-caption: 0.2px;
  --text-subheading: 18px;
  --leading-subheading: 1.4;
  --tracking-subheading: 0.27px;
  --text-heading-sm: 20px;
  --leading-heading-sm: 1.3;
  --tracking-heading-sm: 0.3px;
  --text-heading: 24px;
  --leading-heading: 1.26;
  --tracking-heading: 0.36px;
  --text-heading-lg: 28px;
  --leading-heading-lg: 1.2;
  --tracking-heading-lg: 0.42px;
  --text-display: 48px;
  --leading-display: 1.15;
  --tracking-display: 0.72px;
  --text-display-lg: 72px;
  --leading-display-lg: 1.2;

  /* Typography — Weights */
  --font-weight-regular: 400;
  --font-weight-medium: 500;
  --font-weight-semibold: 600;
  --font-weight-bold: 700;

  /* Spacing */
  --spacing-4: 4px;
  --spacing-5: 5px;
  --spacing-7: 7px;
  --spacing-10: 10px;
  --spacing-14: 14px;
  --spacing-15: 15px;
  --spacing-16: 16px;
  --spacing-20: 20px;
  --spacing-22: 22px;
  --spacing-25: 25px;
  --spacing-30: 30px;
  --spacing-35: 35px;
  --spacing-40: 40px;
  --spacing-50: 50px;
  --spacing-100: 100px;
  --spacing-113: 113px;

  /* Layout */
  --page-max-width: 1200px;
  --section-gap: 64-80px;
  --card-padding: 32-40px;
  --element-gap: 16-24px;

  /* Border Radius */
  --radius-2xl: 16px;
  --radius-2xl-2: 20px;
  --radius-full: 999px;

  /* Named Radii */
  --radius-tags: 999px;
  --radius-cards: 20px;
  --radius-images: 16px;
  --radius-inputs: 16px;
  --radius-buttons: 16px;

  /* Shadows */
  --shadow-sm: rgba(0, 0, 0, 0.2) 0px 1px 4px 0px;
  --shadow-lg: rgba(250, 166, 0, 0.25) 6px 4px 24px 0px;

  /* Surfaces */
  --surface-cream-canvas: #fff8f1;
  --surface-paper-white: #ffffff;
  --surface-orange-brand-surface: #fa5d00;
}
```

### Tailwind v4

```css
@theme {
  /* Colors */
  --color-harvest-flame: #fa5d00;
  --color-marigold-glow: #fee3b5;
  --color-parchment-shadow: #e3d6c5;
  --color-ink-black: #1d1e1c;
  --color-paper-white: #ffffff;
  --color-cream-canvas: #fff8f1;
  --color-mist-gray: #d9d9d9;
  --color-warm-stone: #615f5c;
  --color-driftwood: #8e8b87;
  --color-ironwood: #4a4a47;
  --color-ash: #777571;
  --color-bone: #c0bbb6;
  --color-smoke: #a5a19c;
  --color-graphite: #999999;

  /* Typography */
  --font-muotoweb: 'MuotoWeb', ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
  --font-monarch: 'Monarch', ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;

  /* Typography — Scale */
  --text-caption: 13px;
  --leading-caption: 1.35;
  --tracking-caption: 0.2px;
  --text-subheading: 18px;
  --leading-subheading: 1.4;
  --tracking-subheading: 0.27px;
  --text-heading-sm: 20px;
  --leading-heading-sm: 1.3;
  --tracking-heading-sm: 0.3px;
  --text-heading: 24px;
  --leading-heading: 1.26;
  --tracking-heading: 0.36px;
  --text-heading-lg: 28px;
  --leading-heading-lg: 1.2;
  --tracking-heading-lg: 0.42px;
  --text-display: 48px;
  --leading-display: 1.15;
  --tracking-display: 0.72px;
  --text-display-lg: 72px;
  --leading-display-lg: 1.2;

  /* Spacing */
  --spacing-4: 4px;
  --spacing-5: 5px;
  --spacing-7: 7px;
  --spacing-10: 10px;
  --spacing-14: 14px;
  --spacing-15: 15px;
  --spacing-16: 16px;
  --spacing-20: 20px;
  --spacing-22: 22px;
  --spacing-25: 25px;
  --spacing-30: 30px;
  --spacing-35: 35px;
  --spacing-40: 40px;
  --spacing-50: 50px;
  --spacing-100: 100px;
  --spacing-113: 113px;

  /* Border Radius */
  --radius-2xl: 16px;
  --radius-2xl-2: 20px;
  --radius-full: 999px;

  /* Shadows */
  --shadow-sm: rgba(0, 0, 0, 0.2) 0px 1px 4px 0px;
  --shadow-lg: rgba(250, 166, 0, 0.25) 6px 4px 24px 0px;
}
```
</code></pre></div></div></div></div></div></main></div><script>$RS=function(a,b){a=document.getElementById(a);b=document.getElementById(b);for(a.parentNode.removeChild(a);a.firstChild;)b.parentNode.insertBefore(a.firstChild,b);b.parentNode.removeChild(b)};$RS("S:2","P:2")</script><div hidden id="S:4"><span>Don't use Monarch serif for body text, subheadings, or anything under 48px — it dilutes the hero impact</span></div><script>$RS("S:4","P:4")</script><div hidden id="S:5"><li class="flex items-start gap-2 text-sm text-foreground"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-x mt-0.5 size-4 shrink-0 text-red-500" aria-hidden="true"><path d="M18 6 6 18"></path><path d="m6 6 12 12"></path></svg><span>Don't use sharp 0-4px corner radii on cards or buttons — the 16-20px softness is essential to the warm tactile feel</span></li></div><script>$RS("S:5","P:5")</script><div hidden id="S:6"><li class="flex items-start gap-2 text-sm text-foreground"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-x mt-0.5 size-4 shrink-0 text-red-500" aria-hidden="true"><path d="M18 6 6 18"></path><path d="m6 6 12 12"></path></svg><span>Don't use cool blue-tinted shadows or borders — everything in this system carries a warm undertone</span></li></div><script>$RS("S:6","P:6")</script><div hidden id="S:7"><li class="flex items-start gap-2 text-sm text-foreground"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-x mt-0.5 size-4 shrink-0 text-red-500" aria-hidden="true"><path d="M18 6 6 18"></path><path d="m6 6 12 12"></path></svg><span>Don't apply saturated colors to large background fills — keep the orange small, concentrated, and functional</span></li></div><script>$RS("S:7","P:7")</script><div hidden id="S:8"><li class="flex items-start gap-2 text-sm text-foreground"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-x mt-0.5 size-4 shrink-0 text-red-500" aria-hidden="true"><path d="M18 6 6 18"></path><path d="m6 6 12 12"></path></svg><span>Don't use pure #000000 for text — #1d1e1c (warm near-black) preserves the system's warmth</span></li></div><script>$RS("S:8","P:8")</script><script>$RC("B:1","S:1")</script><script>self.__next_f.push([1,"3c:I[55925,[\"/_next/static/chunks/0mrygax_2m132.js?dpl=dpl_BdwYag37Coka3wCmVQYgfikUc21G\",\"/_next/static/chunks/0d3shmwh5_nmn.js?dpl=dpl_BdwYag37Coka3wCmVQYgfikUc21G\",\"/_next/static/chunks/0w9zxh-w3z4bi.js?dpl=dpl_BdwYag37Coka3wCmVQYgfikUc21G\",\"/_next/static/chunks/023b0pevwkepq.js?dpl=dpl_BdwYag37Coka3wCmVQYgfikUc21G\",\"/_next/static/chunks/11ktc8fnxphx8.js?dpl=dpl_BdwYag37Coka3wCmVQYgfikUc21G\",\"/_next/static/chunks/04eq_ut3lda3~.js?dpl=dpl_BdwYag37Coka3wCmVQYgfikUc21G\",\"/_next/static/chunks/0.jffwitghhk6.js?dpl=dpl_BdwYag37Coka3wCmVQYgfikUc21G\",\"/_next/static/chunks/0b5wrdfrwab.k.js?dpl=dpl_BdwYag37Coka3wCmVQYgfikUc21G\",\"/_next/static/chunks/0i82lysj2jiv0.js?dpl=dpl_BdwYag37Coka3wCmVQYgfikUc21G\"],\"StyleCard\"]\n"])</script><script>self.__next_f.push([1,"39:[\"$\",\"section\",null,{\"className\":\"space-y-6\",\"children\":[[\"$\",\"h2\",null,{\"className\":\"font-heading text-xl font-semibold tracking-heading\",\"children\":\"More like this\"}],[\"$\",\"div\",null,{\"className\":\"grid gap-x-4 gap-y-6 grid-cols-1 sm:grid-cols-2\",\"children\":[[\"$\",\"$L3c\",\"0ab4c544-6147-4998-8365-3a0f6191e54f\",{\"style\":{\"id\":\"0ab4c544-6147-4998-8365-3a0f6191e54f\",\"url\":\"https://www.workable.com\",\"siteName\":\"Workable\",\"screenshotUrl\":\"https://images.refero.design/styles/refero.design/image/76f9e519-613c-4029-973a-c977dee22788.jpg\",\"thumbnailUrl\":\"https://images.refero.design/styles/refero.design/image/4499311c-1a90-4c7c-8316-916a851bedfb.jpg\",\"iconUrl\":\"https://images.refero.design/styles/refero.design/image/44910a4d-586e-4256-989f-eef2504cf263.png\",\"previewVideoUrl\":\"https://images.refero.design/styles/refero.design/video/f07b2e6c-f27c-4a86-a9ff-9c5c5c82cec7.mp4\",\"previewVideoPosterUrl\":\"https://images.refero.design/styles/refero.design/image/6da83b69-5f70-4316-8545-830dd5c0b35f.jpg\",\"previewVideoWidth\":1200,\"previewVideoHeight\":750,\"previewVideoDetailUrl\":\"https://images.refero.design/styles/refero.design/video/62e41a9f-73c2-4b86-a5eb-9d1ed8087126.mp4\",\"previewVideoDetailPosterUrl\":\"https://images.refero.design/styles/refero.design/image/17af07cd-9350-4acf-bdbf-8754e7cca52d.jpg\",\"previewVideoDetailWidth\":1600,\"previewVideoDetailHeight\":1000,\"previewVideoDurationMs\":30984,\"colorScheme\":\"light\",\"colors\":[{\"name\":\"Workable Ink\",\"hex\":\"#0f161e\",\"gradient\":\"$undefined\"},{\"name\":\"Page Canvas\",\"hex\":\"#fbfaf8\",\"gradient\":\"$undefined\"},{\"name\":\"Pure White\",\"hex\":\"#ffffff\",\"gradient\":\"$undefined\"},{\"name\":\"Body Graphite\",\"hex\":\"#3d3e45\",\"gradient\":\"$undefined\"},{\"name\":\"Muted Slate\",\"hex\":\"#6f7073\",\"gradient\":\"$undefined\"},{\"name\":\"Hairline Gray\",\"hex\":\"#efefef\",\"gradient\":\"$undefined\"}],\"fonts\":[\"Proxima Nova\"],\"northStar\":\"warm newsroom with teal ink\",\"managementSignals\":[],\"createdAt\":\"2026-04-30 00:53:19.366382\"},\"compact\":true}],[\"$\",\"$L3c\",\"f4ef80f4-f6e5-4aea-8045-f99efaf208b8\",{\"style\":{\"id\":\"f4ef80f4-f6e5-4aea-8045-f99efaf208b8\",\"url\":\"https://airtable.com\",\"siteName\":\"Airtable\",\"screenshotUrl\":\"https://images.refero.design/styles/refero.design/image/88bcf47d-b43b-4d94-99f6-124d138351d8.jpg\",\"thumbnailUrl\":\"https://images.refero.design/styles/refero.design/image/57e32cc7-07bf-4490-ab6f-c800a5c076b5.jpg\",\"iconUrl\":null,\"previewVideoUrl\":\"https://images.refero.design/styles/refero.design/video/58d6398f-87ed-41d1-b146-ad30b9a23007.mp4\",\"previewVideoPosterUrl\":\"https://images.refero.design/styles/refero.design/image/570efb6b-b9b7-49ef-a9b4-c5060b68a68a.jpg\",\"previewVideoWidth\":1200,\"previewVideoHeight\":750,\"previewVideoDetailUrl\":\"https://images.refero.design/styles/refero.design/video/e1f94f56-62f2-403b-849f-0aa52d767fc5.mp4\",\"previewVideoDetailPosterUrl\":\"https://images.refero.design/styles/refero.design/image/897a7e1d-6c52-47d9-a7c3-6c0f4b9489ef.jpg\",\"previewVideoDetailWidth\":1600,\"previewVideoDetailHeight\":1000,\"previewVideoDurationMs\":17067,\"colorScheme\":\"light\",\"colors\":[{\"name\":\"Parchment Cream\",\"hex\":\"#faf5e8\",\"gradient\":\"$undefined\"},{\"name\":\"Pure White\",\"hex\":\"#ffffff\",\"gradient\":\"$undefined\"},{\"name\":\"Frost White\",\"hex\":\"#f8fafc\",\"gradient\":\"$undefined\"},{\"name\":\"Onyx\",\"hex\":\"#181d26\",\"gradient\":\"$undefined\"},{\"name\":\"Charcoal\",\"hex\":\"#333840\",\"gradient\":\"$undefined\"},{\"name\":\"Graphite\",\"hex\":\"#525965\",\"gradient\":\"$undefined\"}],\"fonts\":[\"Haas Groot Disp\",\"Haas\"],\"northStar\":\"warm workshop with color-coded chapters\",\"managementSignals\":[],\"createdAt\":\"2026-04-12 11:02:27\"},\"compact\":true}],[\"$\",\"$L3c\",\"874aaea0-c718-454e-8a58-f3beed1284ec\",{\"style\":{\"id\":\"874aaea0-c718-454e-8a58-f3beed1284ec\",\"url\":\"https://runway.com\",\"siteName\":\"Runway\",\"screenshotUrl\":\"https://images.refero.design/styles/refero.design/image/4e914c76-ee63-41aa-9da9-729d30b5a241.jpg\",\"thumbnailUrl\":\"https://images.refero.design/styles/refero.design/image/bda9afcb-20b3-49f7-b3ae-70fb79f7a1d5.jpg\",\"iconUrl\":null,\"previewVideoUrl\":null,\"previewVideoPosterUrl\":null,\"previewVideoWidth\":null,\"previewVideoHeight\":null,\"previewVideoDetailUrl\":null,\"previewVideoDetailPosterUrl\":null,\"previewVideoDetailWidth\":null,\"previewVideoDetailHeight\":null,\"previewVideoDurationMs\":null,\"colorScheme\":\"light\",\"colors\":[{\"name\":\"Cream Canvas\",\"hex\":\"#f8f7f5\",\"gradient\":\"$undefined\"},{\"name\":\"Pure Paper\",\"hex\":\"#ffffff\",\"gradient\":\"$undefined\"},{\"name\":\"Linen Border\",\"hex\":\"#e3dfd5\",\"gradient\":\"$undefined\"},{\"name\":\"Stone Mist\",\"hex\":\"#d5d2cd\",\"gradient\":\"$undefined\"},{\"name\":\"Warm Ash\",\"hex\":\"#aca89f\",\"gradient\":\"$undefined\"},{\"name\":\"Driftwood\",\"hex\":\"#8f897e\",\"gradient\":\"$undefined\"}],\"fonts\":[\"Interphases Pro Variable\"],\"northStar\":\"Kraft paper ledger under amber desk lamp. Every screen should feel like opening a well-organized financial notebook: cream paper, espresso ink, one warm highlight color, no cold digital surfaces.\",\"managementSignals\":[],\"createdAt\":\"2026-04-30 00:34:57.777204\"},\"compact\":true}],\"$L3d\",\"$L3e\",\"$L3f\",\"$L40\",\"$L41\",\"$L42\",\"$L43\",\"$L44\",\"$L45\",\"$L46\",\"$L47\",\"$L48\",\"$L49\",\"$L4a\",\"$L4b\",\"$L4c\",\"$L4d\"]}]]}]\n"])</script><script>self.__next_f.push([1,"3d:[\"$\",\"$L3c\",\"3e100552-a8ad-4179-b89a-6aa5113b92e1\",{\"style\":{\"id\":\"3e100552-a8ad-4179-b89a-6aa5113b92e1\",\"url\":\"https://www.hubspot.com\",\"siteName\":\"HubSpot\",\"screenshotUrl\":\"https://images.refero.design/styles/refero.design/image/e56a8496-34f9-4876-bfa0-aee058d38d18.jpg\",\"thumbnailUrl\":\"https://images.refero.design/styles/refero.design/image/1a9bb07a-02e4-4bff-a8a0-9d7d85119bd4.jpg\",\"iconUrl\":null,\"previewVideoUrl\":\"https://images.refero.design/styles/refero.design/video/3e4191bd-d164-423e-a9ad-8493f7a5cb9c.mp4\",\"previewVideoPosterUrl\":\"https://images.refero.design/styles/refero.design/image/e8046d0c-a0b8-4201-9438-67556c4e5169.jpg\",\"previewVideoWidth\":1200,\"previewVideoHeight\":750,\"previewVideoDetailUrl\":\"https://images.refero.design/styles/refero.design/video/c60350e0-4440-4241-a9f9-b648a9be28ed.mp4\",\"previewVideoDetailPosterUrl\":\"https://images.refero.design/styles/refero.design/image/69f38652-e3f4-4163-9eb1-0f21e5c2f89b.jpg\",\"previewVideoDetailWidth\":1600,\"previewVideoDetailHeight\":1000,\"previewVideoDurationMs\":16000,\"colorScheme\":\"light\",\"colors\":[{\"name\":\"Sprout Orange\",\"hex\":\"#ff4800\",\"gradient\":\"$undefined\"},{\"name\":\"Canvas Cream\",\"hex\":\"#fcfcfa\",\"gradient\":\"$undefined\"},{\"name\":\"Warm Parchment\",\"hex\":\"#f8f5ee\",\"gradient\":\"$undefined\"},{\"name\":\"Ink\",\"hex\":\"#1f1f1f\",\"gradient\":\"$undefined\"},{\"name\":\"Pure Black\",\"hex\":\"#000000\",\"gradient\":\"$undefined\"},{\"name\":\"Graphite\",\"hex\":\"#60605f\",\"gradient\":\"$undefined\"}],\"fonts\":[\"HubSpot Sans\",\"HubSpot Serif\",\"HubSpot Serif Page Header Human\"],\"northStar\":\"Warm cream paper with a single orange spark. HubSpot feels like a design magazine printed on heavy stock — editorial serif headlines, warm off-white pages, and one flame-orange accent that lights up only the moments that matter.\",\"managementSignals\":[],\"createdAt\":\"2026-04-30 01:01:46.488613\"},\"compact\":true}]\n"])</script><script>self.__next_f.push([1,"3e:[\"$\",\"$L3c\",\"e8589e7c-5ba9-4923-aa7f-0f1bf0d679be\",{\"style\":{\"id\":\"e8589e7c-5ba9-4923-aa7f-0f1bf0d679be\",\"url\":\"https://campsite.design\",\"siteName\":\"Campsite\",\"screenshotUrl\":\"https://images.refero.design/styles/refero.design/image/9a707304-ad05-4c60-9515-6f9ce7ff8070.jpg\",\"thumbnailUrl\":\"https://images.refero.design/styles/refero.design/image/35608325-9d9d-434a-a3ac-70848a70ed1f.jpg\",\"iconUrl\":null,\"previewVideoUrl\":\"https://images.refero.design/styles/refero.design/video/27ecf6aa-60c7-4b6f-95d6-b205fe6c7801.mp4\",\"previewVideoPosterUrl\":\"https://images.refero.design/styles/refero.design/image/41d0635a-c9f7-4319-9cf0-f1a83a5bf34c.jpg\",\"previewVideoWidth\":1200,\"previewVideoHeight\":750,\"previewVideoDetailUrl\":\"https://images.refero.design/styles/refero.design/video/e7acf76d-c172-4839-b43e-7c8ec103914b.mp4\",\"previewVideoDetailPosterUrl\":\"https://images.refero.design/styles/refero.design/image/04d5a5b9-ad96-4a53-a8f7-4d782391e94d.jpg\",\"previewVideoDetailWidth\":1600,\"previewVideoDetailHeight\":1000,\"previewVideoDurationMs\":16680,\"colorScheme\":\"light\",\"colors\":[{\"name\":\"Campfire Orange\",\"hex\":\"#ff6b1a\",\"gradient\":\"$undefined\"},{\"name\":\"Ember Brown\",\"hex\":\"#451a03\",\"gradient\":\"$undefined\"},{\"name\":\"Sunlit Cream\",\"hex\":\"#fef3c7\",\"gradient\":\"$undefined\"},{\"name\":\"Forest Pulse\",\"hex\":\"#22c55e\",\"gradient\":\"$undefined\"},{\"name\":\"Ember Alert\",\"hex\":\"#ef4444\",\"gradient\":\"$undefined\"},{\"name\":\"Midnight Ink\",\"hex\":\"#171717\",\"gradient\":\"$undefined\"}],\"fonts\":[\"Inter\",\"ui-monospace\",\"emoji\"],\"northStar\":\"sunlit editorial workspace — warm cream paper with one orange stamp of intent\",\"managementSignals\":[],\"createdAt\":\"2026-02-02 20:17:29\"},\"compact\":true}]\n"])</script><script>self.__next_f.push([1,"3f:[\"$\",\"$L3c\",\"f3c955e4-0fea-462d-b05f-868552e9628c\",{\"style\":{\"id\":\"f3c955e4-0fea-462d-b05f-868552e9628c\",\"url\":\"https://ambrook.com\",\"siteName\":\"Ambrook\",\"screenshotUrl\":\"https://images.refero.design/styles/refero.design/image/9db9ce24-156c-4f68-81a9-4bd775d22094.jpg\",\"thumbnailUrl\":\"https://images.refero.design/styles/refero.design/image/e91f796c-8197-4cf6-82c5-861ca311310f.jpg\",\"iconUrl\":\"https://images.refero.design/styles/refero.design/image/8c393409-eedb-440e-974f-286043aaf4b9.png\",\"previewVideoUrl\":\"https://images.refero.design/styles/refero.design/video/b91a639f-cc74-475f-8567-87deaabd7249.mp4\",\"previewVideoPosterUrl\":\"https://images.refero.design/styles/refero.design/image/831f7016-d296-4b7b-b8d0-3fe9558a42bd.jpg\",\"previewVideoWidth\":1200,\"previewVideoHeight\":750,\"previewVideoDetailUrl\":\"https://images.refero.design/styles/refero.design/video/ff3e7a63-dbd6-44a9-b328-f7e49c7fa342.mp4\",\"previewVideoDetailPosterUrl\":\"https://images.refero.design/styles/refero.design/image/cfbe474b-2de0-425d-8176-5fd620cfa15f.jpg\",\"previewVideoDetailWidth\":1600,\"previewVideoDetailHeight\":1000,\"previewVideoDurationMs\":21167,\"colorScheme\":\"light\",\"colors\":[{\"name\":\"Parchment\",\"hex\":\"#fcfaf1\",\"gradient\":\"$undefined\"},{\"name\":\"Bone\",\"hex\":\"#efe9e0\",\"gradient\":\"$undefined\"},{\"name\":\"Pure White\",\"hex\":\"#ffffff\",\"gradient\":\"$undefined\"},{\"name\":\"Loam\",\"hex\":\"#c7bcaf\",\"gradient\":\"$undefined\"},{\"name\":\"Bark\",\"hex\":\"#96897b\",\"gradient\":\"$undefined\"},{\"name\":\"Saddle\",\"hex\":\"#50463c\",\"gradient\":\"$undefined\"}],\"fonts\":[\"Lateral\",\"Lateral Narrow\",\"Lateral Display\"],\"northStar\":\"harvest ledger on butcher paper\",\"managementSignals\":[],\"createdAt\":\"2026-05-10 23:14:49.393526\"},\"compact\":true}]\n"])</script><script>self.__next_f.push([1,"40:[\"$\",\"$L3c\",\"dfbcffc2-79a3-4349-b5c6-1aa9fae4fcf4\",{\"style\":{\"id\":\"dfbcffc2-79a3-4349-b5c6-1aa9fae4fcf4\",\"url\":\"https://getapron.com\",\"siteName\":\"Automate Supplier Payments\",\"screenshotUrl\":\"https://images.refero.design/styles/refero.design/image/0b089746-fe7e-4a86-9b7a-532d40b01377.jpg\",\"thumbnailUrl\":\"https://images.refero.design/styles/refero.design/image/c4438333-b100-4473-a0f2-807e822343e5.jpg\",\"iconUrl\":\"https://images.refero.design/styles/refero.design/image/c0c0ac2e-d2f2-4b9b-9049-682591dee55c.png\",\"previewVideoUrl\":\"https://images.refero.design/styles/refero.design/video/c02c6f05-9742-4739-9fcb-c97e523641e9.mp4\",\"previewVideoPosterUrl\":\"https://images.refero.design/styles/refero.design/image/887619c5-620e-4abc-94d9-ab46d8b8d153.jpg\",\"previewVideoWidth\":1200,\"previewVideoHeight\":750,\"previewVideoDetailUrl\":\"https://images.refero.design/styles/refero.design/video/62eb0b55-9c4b-42a5-9acc-dc8e558787f0.mp4\",\"previewVideoDetailPosterUrl\":\"https://images.refero.design/styles/refero.design/image/57249002-0de2-4431-b85b-a47fbb25e9a0.jpg\",\"previewVideoDetailWidth\":1600,\"previewVideoDetailHeight\":1000,\"previewVideoDurationMs\":20400,\"colorScheme\":\"light\",\"colors\":[{\"name\":\"Buttercream\",\"hex\":\"#fff6d2\",\"gradient\":\"$undefined\"},{\"name\":\"Marigold\",\"hex\":\"#ffd801\",\"gradient\":\"$undefined\"},{\"name\":\"Ink Black\",\"hex\":\"#000000\",\"gradient\":\"$undefined\"},{\"name\":\"Bone White\",\"hex\":\"#ffffff\",\"gradient\":\"$undefined\"},{\"name\":\"Char\",\"hex\":\"#666664\",\"gradient\":\"$undefined\"},{\"name\":\"Oat\",\"hex\":\"#cccbc7\",\"gradient\":\"$undefined\"}],\"fonts\":[\"sans-serif\",\"Champ\",\"DM Sans\",\"DM Mono\",\"Arial\"],\"northStar\":\"butcher paper bakery ledger.\\n\\nA cream-colored, sun-warmed workspace where thick slab type, pill buttons, and a single school-bus yellow accent do all the work — no shadows, no gradients, just warm paper and confident black ink.\",\"managementSignals\":[],\"createdAt\":\"2026-05-07 22:01:44.109334\"},\"compact\":true}]\n"])</script><script>self.__next_f.push([1,"41:[\"$\",\"$L3c\",\"db451eca-8de6-43a9-a5d5-35271befdffd\",{\"style\":{\"id\":\"db451eca-8de6-43a9-a5d5-35271befdffd\",\"url\":\"https://www.amplemarket.com\",\"siteName\":\"Amplemarket\",\"screenshotUrl\":\"https://images.refero.design/styles/refero.design/image/50b38758-7635-45f5-b814-36a392e3f2f9.jpg\",\"thumbnailUrl\":\"https://images.refero.design/styles/refero.design/image/687b6703-a095-45ab-a973-81589b06a886.jpg\",\"iconUrl\":\"https://images.refero.design/styles/refero.design/image/316138b5-fe6e-4d9c-a15c-b29c1fc47999.png\",\"previewVideoUrl\":\"https://images.refero.design/styles/refero.design/video/593cb117-9f72-4d8e-b894-1f8f21bb1fdf.mp4\",\"previewVideoPosterUrl\":\"https://images.refero.design/styles/refero.design/image/0a26919b-1e70-497a-b634-6c5a1ac6c881.jpg\",\"previewVideoWidth\":1200,\"previewVideoHeight\":750,\"previewVideoDetailUrl\":\"https://images.refero.design/styles/refero.design/video/72f102c7-dd43-4e3c-b86f-78e5fc068d77.mp4\",\"previewVideoDetailPosterUrl\":\"https://images.refero.design/styles/refero.design/image/10872d6a-0e01-4890-9830-99bb07cd9ad4.jpg\",\"previewVideoDetailWidth\":1600,\"previewVideoDetailHeight\":1000,\"previewVideoDurationMs\":33434,\"colorScheme\":\"light\",\"colors\":[{\"name\":\"Phoenix Orange\",\"hex\":\"#e8400d\",\"gradient\":\"radial-gradient(386.06% 162.79% at 3.76985% -12.1005%, rgb(232, 64, 13) 0%, rgb(255, 238, 216) 31.14%, rgb(208, 178, 255) 81.98%)\"},{\"name\":\"Midnight Indigo\",\"hex\":\"#10054d\",\"gradient\":\"$unde