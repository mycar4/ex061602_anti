name: Mobility Excellence System
colors:
  surface: '#f3faff'
  surface-dim: '#c7dde9'
  surface-bright: '#f3faff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#e6f6ff'
  surface-container: '#dbf1fe'
  surface-container-high: '#d5ecf8'
  surface-container-highest: '#cfe6f2'
  on-surface: '#071e27'
  on-surface-variant: '#414752'
  inverse-surface: '#1e333c'
  inverse-on-surface: '#dff4ff'
  outline: '#717783'
  outline-variant: '#c1c6d4'
  surface-tint: '#005faf'
  primary: '#005dac'
  on-primary: '#ffffff'
  primary-container: '#1976d2'
  on-primary-container: '#fffdff'
  inverse-primary: '#a5c8ff'
  secondary: '#795900'
  on-secondary: '#ffffff'
  secondary-container: '#ffbf00'
  on-secondary-container: '#6d5000'
  tertiary: '#505e68'
  on-tertiary: '#ffffff'
  tertiary-container: '#697781'
  on-tertiary-container: '#fdfdff'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#d4e3ff'
  primary-fixed-dim: '#a5c8ff'
  on-primary-fixed: '#001c3a'
  on-primary-fixed-variant: '#004786'
  secondary-fixed: '#ffdfa0'
  secondary-fixed-dim: '#fbbc00'
  on-secondary-fixed: '#261a00'
  on-secondary-fixed-variant: '#5c4300'
  tertiary-fixed: '#d6e5ef'
  tertiary-fixed-dim: '#bac9d3'
  on-tertiary-fixed: '#0f1d25'
  on-tertiary-fixed-variant: '#3b4951'
  background: '#f3faff'
  on-background: '#071e27'
  surface-variant: '#cfe6f2'
typography:
  display-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 40px
    fontWeight: '800'
    lineHeight: 48px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
  headline-lg-mobile:
    fontFamily: Plus Jakarta Sans
    fontSize: 26px
    fontWeight: '700'
    lineHeight: 32px
  headline-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '500'
    lineHeight: 28px
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-lg:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '600'
    lineHeight: 20px
  data-numeric:
    fontFamily: Plus Jakarta Sans
    fontSize: 22px
    fontWeight: '700'
    lineHeight: 28px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 8px
  touch-target-min: 48px
  gutter-mobile: 16px
  gutter-desktop: 24px
  margin-edge: 20px
  stack-sm: 12px
  stack-md: 24px
---

## Brand & Style

The design system is engineered for the professional driver, balancing data-driven precision with the warmth of a supportive partner. The brand personality is an **Expert Ally**: highly tech-savvy and reliable, yet encouraging and "luck-bringing" through its gamified success metrics.

The visual style follows a **Modern-Tactile** approach. It leverages clean, spacious layouts (Modernism) to ensure information density never leads to cognitive overload, while utilizing soft gradients and subtle depth (Tactile) to make the interface feel responsive and friendly. This combination evokes an emotional response of security and optimism—essential for users who spend long hours on the road.

Key stylistic pillars:
- **Calm Clarity:** High-legibility layouts that reduce visual noise.
- **Optimistic Precision:** Using vibrant accents to highlight profit and success.
- **Dynamic Utility:** Large interactive surfaces optimized for in-vehicle mounting and quick interactions.

## Colors

The palette is strategically chosen to accommodate the unique environment of a taxi cabin, where lighting conditions vary drastically.

- **Primary (Trust Blue):** Used for primary actions and core navigation. It provides high contrast against light backgrounds while remaining professional.
- **Secondary (Daetong Gold):** Reserved for "luck" moments, profit indicators, and achievement rewards. This color represents wealth and positive outcomes.
- **Tertiary (Calm Surface):** A soft, desaturated pastel blue used for large background areas and card surfaces. It significantly reduces white-point glare, preventing eye strain during night shifts.
- **Neutral (Slate Gray):** Provides grounding and clear hierarchy for secondary information and body text.

**State Tokens:**
- **Success:** #4CAF50 (Clear green for completed fares).
- **Surface:** #F8FAFC (Ultra-light gray for layout differentiation).
- **Warning:** #FF7043 (Soft orange for traffic or safety alerts).

## Typography

This design system uses a dual-font strategy to balance character with utility.

**Plus Jakarta Sans** is the headline face. Its open apertures and friendly curves make large titles feel approachable while maintaining a modern, tech-forward aesthetic. It is also used for key data points (like earnings) to give them a distinct, impactful personality.

**Inter** is the functional workhorse. It is utilized for all body copy, UI labels, and lists. Its neutral, systematic design ensures maximum legibility at smaller sizes, especially when viewed at arm's length on a dashboard mount.

**Hierarchy Rules:**
- Use **Bold/Extrabold** for all monetary values to ensure they are glanceable.
- Desktop headings scale down by 20% for mobile to prevent text wrapping that disrupts layout flow.
- Maintain a minimum body size of 16px to support accessibility for older demographics.

## Layout & Spacing

The layout is **Mobile-First**, utilizing a 4-column grid for phone screens and a 12-column grid for tablet/desktop dashboards. The system relies on a **strict 8px spacing rhythm** to maintain visual consistency.

**Tap-ability & Ergonomics:**
- All primary interactive elements must adhere to a minimum **48px touch target**.
- Frequent actions are placed in the "Bottom-Reach Zone" for easier one-handed use during stops.
- Content is housed in cards with defined vertical stacks (`stack-md`) to ensure the driver can easily distinguish between different data groups (e.g., current fare vs. daily earnings).

**Adaptive Reflow:**
- On mobile, cards span the full width minus the `margin-edge`.
- On desktop, cards are arranged in a masonry or dashboard grid, allowing for simultaneous viewing of the map and data reports.

## Elevation & Depth

To convey hierarchy without overwhelming the user with shadows, this design system employs **Tonal Layering** combined with soft, directional light.

1.  **Base (Level 0):** The primary background, colored in `tertiary_color_hex` (Pastel Blue) to keep the overall UI calm.
2.  **Surface (Level 1):** White or light-gray cards. These use a very soft, diffused shadow (10% opacity, 8px blur) to appear slightly lifted.
3.  **Active/Floating (Level 2):** Primary buttons and active selection states. These feature a stronger shadow and a 1px inner border to simulate a "tappable" physical button.
4.  **Glass Overlay:** Used for non-modal notifications or dashboard overlays. A subtle backdrop blur (12px) ensures the map or background data remains visible but legible.

This tiered approach ensures that the most important information—the "now" tasks—literally sits on top of the historical data.

## Shapes

The shape language is **Rounded**, echoing the friendly and supportive nature of the brand.

- **Standard Components:** Buttons and input fields use a **0.5rem (8px)** corner radius.
- **Large Components:** Cards and major containers use a **1rem (16px)** radius (`rounded-lg`) to create a soft, modern frame for content.
- **Pill Shapes:** Used exclusively for status indicators (e.g., "Active," "Completed") and chips to differentiate them from actionable buttons.

Avoid sharp 90-degree corners to maintain the approachable, non-intimidating "consultant" persona of the platform.

## Components

**Buttons:**
- **Primary:** High-contrast Trust Blue with white text. Height: 56px for maximum tap-ability.
- **Secondary/Action:** Amber Gold with dark slate text. Used for "Claim Reward" or "Start Shift."
- **Ghost:** Transparent with a 2px border for less critical actions.

**Cards:**
- All cards feature a white background against the pastel blue layout.
- Include a 1px stroke (#E2E8F0) for crispness.
- Use internal padding of 20px to keep data points from feeling cramped.

**Data Visualization:**
- Charts should use the `secondary_color_hex` for "Good/Profit" trends and a muted neutral for historical data.
- Use thick lines (3px+) in line charts for visibility while driving.

**Input Fields:**
- Large text inputs with clear floating labels.
- Focus states must use a 3px Amber Gold ring to provide unmistakable visual feedback.

**Community Chips:**
- Interactive tags for the forum or community section should have a 32px height and use light tonal backgrounds to differentiate between "Question," "Tip," and "Success Story."