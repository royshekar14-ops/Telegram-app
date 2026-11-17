---
name: Obsidian Violet Unlock
colors:
  surface: '#13121c'
  surface-dim: '#13121c'
  surface-bright: '#393843'
  surface-container-lowest: '#0d0d16'
  surface-container-low: '#1b1b24'
  surface-container: '#1f1f28'
  surface-container-high: '#292933'
  surface-container-highest: '#34343e'
  on-surface: '#e4e1ee'
  on-surface-variant: '#cbc3d7'
  inverse-surface: '#e4e1ee'
  inverse-on-surface: '#302f3a'
  outline: '#958ea0'
  outline-variant: '#494454'
  surface-tint: '#d0bcff'
  primary: '#d0bcff'
  on-primary: '#3c0091'
  primary-container: '#a078ff'
  on-primary-container: '#340080'
  inverse-primary: '#6d3bd7'
  secondary: '#4edea3'
  on-secondary: '#003824'
  secondary-container: '#00a572'
  on-secondary-container: '#00311f'
  tertiary: '#ffb95f'
  on-tertiary: '#472a00'
  tertiary-container: '#ca8100'
  on-tertiary-container: '#3e2400'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#e9ddff'
  primary-fixed-dim: '#d0bcff'
  on-primary-fixed: '#23005c'
  on-primary-fixed-variant: '#5516be'
  secondary-fixed: '#6ffbbe'
  secondary-fixed-dim: '#4edea3'
  on-secondary-fixed: '#002113'
  on-secondary-fixed-variant: '#005236'
  tertiary-fixed: '#ffddb8'
  tertiary-fixed-dim: '#ffb95f'
  on-tertiary-fixed: '#2a1700'
  on-tertiary-fixed-variant: '#653e00'
  background: '#13121c'
  on-background: '#e4e1ee'
  surface-variant: '#34343e'
typography:
  headline-xl:
    fontFamily: Inter
    fontSize: 36px
    fontWeight: '800'
    lineHeight: 44px
  headline-xl-mobile:
    fontFamily: Inter
    fontSize: 28px
    fontWeight: '800'
    lineHeight: 34px
  headline-lg:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '700'
    lineHeight: 32px
  headline-sm:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 26px
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  body-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '400'
    lineHeight: 16px
  label-lg:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '600'
    lineHeight: 18px
  label-md:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
  label-sm:
    fontFamily: Inter
    fontSize: 10px
    fontWeight: '700'
    lineHeight: 12px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  gutter: 1rem
  margin: 1rem
  space-xs: 0.25rem
  space-sm: 0.5rem
  space-md: 1rem
  space-lg: 1.5rem
  space-xl: 2rem
---

## Brand & Style
The design system establishes a premium, gamified, and hyper-focused mobile experience engineered specifically for the Telegram Mini App (TMA) runtime. It targets tech-literate, digital-native media consumers who unlock exclusive video streaming, community content, and premium files via bot micro-tasks and rewards. 

The aesthetic is a hybrid of **Deep Slate Glassmorphism** and **Electric Neon Cyber-Modernism**. Deep midnight backdrops eliminate optical glare in low-light environments, while high-octane violet gradients guide visual attention effortlessly toward primary unlock CTAs and verification status nodes. Micro-interactions evoke immediate tactile satisfaction through luminous glowing states, crisp border illumination, and low-latency feedback.

## Colors
The palette balances immersive dark values with high-intensity chromatic focal points:
- **Base Cavities & Surfaces:** Base canvas sits at deep obsidian `#0B0B14`, stepped up to elevated slate `#121124` for card trays, and `#1E1B3A` for nested containers and modal sheets.
- **Electric Purples (Action Core):** The primary interaction spectrum spans vibrant `#8B5CF6`, commanding `#6D28D9`, and deep perimeter `#4C1D95`. Gradients flow at a 135° diagonal from `#8B5CF6` to `#6D28D9` for high-conversion actions.
- **Luminous Emerald (Task Progression):** Status milestones, completed task verifications, and success notifications leverage `#10B981` with an inner anchor of `#059669`.
- **Radiant Gold (Rewards & Multipliers):** Token bonuses, unlock keys, and premium stars resolve to `#F59E0B`.
- **Text & Stroke Contrast:** Primary typography employs pure crisp `#FFFFFF`, secondary data tokens use `#94A3B8`, and structural borders use translucent violet-tinted lines (`rgba(139, 92, 246, 0.15)`).

## Typography
Typographic clarity relies on the tight, neutral geometry of **Inter**. In native mobile WebViews, fallback is delegated to `-apple-system, BlinkMacSystemFont, "SF Pro Display"`.

- **Letter-Spacing Metrics:** Display headlines (`headline-xl`, `headline-lg`) feature tracking tightened to `-0.02em` to project authority and precision. Micro-labels (`label-sm`, `label-md`) use uppercase tracking pushed out to `+0.05em` to ensure instant scanability on mobile screens under variable ambient light.
- **Tabular Numerals:** For real-time unlock count-ups, countdown timers, and reward tallying, activate CSS `font-variant-numeric: tabular-nums` to eliminate jitter across data updates.

## Layout & Spacing
The layout implements a mobile-first fluid single-column structure calibrated directly for the constrained Telegram Mini App canvas:
- **Canvas Constraints:** Maximum viewport width locks to `480px` on desktop clients, centered with dark margins. On mobile handheld devices, width expands fluidly to `100%`.
- **Viewport Safe Insets:** All root containers must account for native TMA chrome, padding top navigation against Telegram’s top bar (`var(--tg-viewport-height)` / safe-area-inset-top) and reserving bottom clearance for floating actions (`env(safe-area-inset-bottom, 16px)`).
- **Rhythm & Stacking:** Micro component separations stick to `space-xs` (4px) and `space-sm` (8px). Structural groupings, card content lists, and step sequences default to `space-md` (16px) gutters. Section transitions utilize `space-xl` (32px).

## Elevation & Depth
Depth is realized through a layered composite of **translucent dark glass** and **luminous chromatic backlights**:
- **Layer 0 (Canvas):** Solid `#0B0B14`.
- **Layer 1 (Subdued Glass Containers):** Background fill of `rgba(18, 17, 36, 0.72)` paired with `backdrop-filter: blur(16px)` and an ultra-subtle perimeter stroke of `1px solid rgba(255, 255, 255, 0.08)`.
- **Layer 2 (Elevated & Active Items):** Background fill of `rgba(30, 27, 58, 0.85)` paired with `backdrop-filter: blur(24px)` and a glowing stroke of `1px solid rgba(139, 92, 246, 0.35)`.
- **Luminous Drop Glows:** Elevated cards under active unlock states emit an ambient halo using `box-shadow: 0px 10px 30px -5px rgba(109, 40, 217, 0.3)`. Primary action buttons carry a focused interactive under-glow: `0px 4px 20px 0px rgba(139, 92, 246, 0.45)`.
- **Completed Success Sheen:** Verified components transition their border to `rgba(16, 185, 129, 0.4)` accompanied by a subtle `0px 4px 20px rgba(16, 185, 129, 0.2)` soft glow.

## Shapes
The design system adopts a **Rounded** posture (`roundedness: 2`):
- Base interactive controls and inputs sit at `0.5rem` (8px).
- Content cards, modal sheets, and video thumbnail wrappers leverage `rounded-lg` (`1rem` / 16px).
- Parent container modules and floating action overlays leverage `rounded-xl` (`1.5rem` / 24px).
- Progress rings, profile avatars, status indicators, and pill badges break out of the scale to use absolute full radii (`9999px`).

## Components

### Buttons
- **Primary CTA ("Unlock Video"):** Styled with an electric gradient background (`linear-gradient(135deg, #8B5CF6 0%, #6D28D9 100%)`), crisp white `label-lg` typography, `0.5rem` corner radius, and an ambient purple drop glow. On tap, scales to `0.98` with haptic feedback trigger.
- **Secondary / Task Action:** Glass fill `rgba(139, 92, 246, 0.12)`, border `1px solid rgba(139, 92, 246, 0.3)`, text `#8B5CF6`.
- **Completed / Disabled:** Subdued slate fill `rgba(255, 255, 255, 0.05)`, border `1px solid rgba(255, 255, 255, 0.08)`, text `#64748B`.

### Video Unlock Glass Cards
- Built with Layer 1 glassmorphism: `1rem` radius, 16px internal padding, `1px solid rgba(255, 255, 255, 0.08)`.
- Video previews feature a 16:9 blurred backdrop thumbnail overlaid with a translucent violet scrim, a locked padlock indicator, and total duration badge.

### Circular Progress Rings
- SVG-based circular meters tracking prerequisite step completions (e.g., "2 of 3 tasks done").
- Track path: `rgba(255, 255, 255, 0.08)`, stroke width 6px.
- Value path: High-visibility electric purple `#8B5CF6` terminating with a soft round cap, shifting dynamically to `#10B981` upon reaching 100%. Center area houses numeric label or unlock icon.

### Task List Items & Step Nodes
- Horizontal row layouts (`space-md` height) with left-aligned task icon, central title/subtitle stack, and right-aligned action trigger.
- Pending state: Outlined circle or arrow affordance.
- Completed state: `#10B981` filled circle containing a crisp white checkmark, accompanied by a faint emerald background sheen across the row.

### Badges & Chips
- **Reward Multipliers:** Background `rgba(245, 158, 11, 0.15)`, text `#F59E0B`, border `1px solid rgba(245, 158, 11, 0.3)`.
- **Status Pills:** Background `rgba(16, 185, 129, 0.15)`, text `#10B981`, border `1px solid rgba(16, 185, 129, 0.3)`.
- Formatted with `label-sm`, uppercase tracking, pill roundedness (`9999px`), and 4px vertical / 8px horizontal padding.

### Checkboxes & Radio Selection
- 20x20px dimension with 6px corner radius for checkboxes, full circle for radios.
- Unchecked: Slate cavity fill with `1px solid rgba(255, 255, 255, 0.2)`.
- Checked: Electric violet gradient fill, elevated center white iconography, and subtle violet halo.

### Input Fields (Verification Keys & Referrals)
- Height fixed to 48px, background `rgba(18, 17, 36, 0.9)`, border `1px solid rgba(255, 255, 255, 0.12)`, radius `0.5rem`.
- Focus state activates a vivid `#8B5CF6` stroke and ambient outer shadow ring. Includes a built-in "Paste" micro-action pill on the trailing edge.