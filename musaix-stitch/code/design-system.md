---
name: Sonic Precision
colors:
  surface: '#131313'
  surface-dim: '#131313'
  surface-bright: '#3a3939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1c1b1b'
  surface-container: '#201f1f'
  surface-container-high: '#2a2a2a'
  surface-container-highest: '#353534'
  on-surface: '#e5e2e1'
  on-surface-variant: '#b9cacb'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#849495'
  outline-variant: '#3a494b'
  surface-tint: '#00dbe7'
  primary: '#e1fdff'
  on-primary: '#00363a'
  primary-container: '#00f2ff'
  on-primary-container: '#006a71'
  inverse-primary: '#00696f'
  secondary: '#d7ffc5'
  on-secondary: '#053900'
  secondary-container: '#2ff801'
  on-secondary-container: '#0f6d00'
  tertiary: '#fff4f9'
  on-tertiary: '#5b005b'
  tertiary-container: '#ffcbf4'
  on-tertiary-container: '#ab00aa'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#74f5ff'
  primary-fixed-dim: '#00dbe7'
  on-primary-fixed: '#002022'
  on-primary-fixed-variant: '#004f54'
  secondary-fixed: '#79ff5b'
  secondary-fixed-dim: '#2ae500'
  on-secondary-fixed: '#022100'
  on-secondary-fixed-variant: '#095300'
  tertiary-fixed: '#ffd7f5'
  tertiary-fixed-dim: '#ffabf3'
  on-tertiary-fixed: '#380038'
  on-tertiary-fixed-variant: '#810081'
  background: '#131313'
  on-background: '#e5e2e1'
  surface-variant: '#353534'
typography:
  headline-xl:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '800'
    lineHeight: 56px
    letterSpacing: 0.05em
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: 0.02em
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
    letterSpacing: 0.01em
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-sm:
    fontFamily: Geist
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
    letterSpacing: 0.08em
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 28px
    fontWeight: '700'
    lineHeight: 36px
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 4px
  gutter: 16px
  margin-mobile: 16px
  margin-desktop: 40px
  container-max: 1440px
---

## Brand & Style

The design system is engineered for the high-performance world of professional music production. It targets technical creators who require a focused, low-distraction environment that remains visually stimulating during long studio sessions. 

The aesthetic is a fusion of **High-Tech Minimalism** and **Glassmorphism**. It leverages a "Dark Mode First" philosophy to reduce eye strain, using deep obsidian surfaces punctuated by vibrant, "active-light" accents that mimic the glowing LEDs of premium hardware synths. The emotional response is one of surgical precision, modern sophistication, and creative energy.

## Colors

This design system utilizes a high-contrast dark palette to establish a clear visual hierarchy within complex audio interfaces.

- **Primary (#00F2FF):** Reserved for interactive states, primary actions, and "on" signals. Use with a soft outer glow to simulate a light-emitting source.
- **Secondary (#39FF14):** Indicates active processing engines, "signal-ok" states, and secondary rhythmic indicators.
- **Tertiary (#FF00FF):** Used sparingly for peak alerts, critical system warnings, or "destructive" actions (like deleting a track).
- **Backgrounds:** The foundation is a pure Deep Obsidian (#0A0A0A). Layered surfaces use Dark Slate (#1A1A1A) to provide depth without breaking the dark aesthetic.
- **Typography:** Headlines are rendered in pure White for maximum punch; body text uses Silver (#C0C0C0) to lower the visual noise of dense instructional content.

## Typography

The typography system prioritizes legibility and a "technical" feel. 

- **Headlines:** Utilize **Inter** with heavy weights (700-800) and increased letter-spacing (tracking). This creates a rhythmic, modular look that feels architectural.
- **Body:** Standard **Inter** is used for its exceptional clarity in low-light environments.
- **Labels:** The **Geist** font is introduced for UI labels and metadata. Its monospaced-adjacent proportions complement the music production theme, suggesting data and parameters. Labels should almost always be uppercase with wide tracking for a professional "meter-label" look.

## Layout & Spacing

The layout follows a **Fluid Grid** model based on a 4px baseline unit, ensuring all elements align to a technical rhythm.

- **Desktop:** A 12-column grid with 16px gutters. Margins are generous (40px) to give the complex UI "room to breathe."
- **Mobile:** A 4-column grid with 16px margins.
- **Logic:** Information density is high. Use padding to group related parameters (e.g., ADSR envelope controls) within distinct containers. Spacing should be used to create clear separation between the global navigation, the track workspace, and the detail inspector panels.

## Elevation & Depth

Depth is not communicated through traditional shadows, but through **Tonal Layering** and **Minimalist Outlines**.

- **Surfaces:** Use 1px solid borders (#333) to define card boundaries against the #0A0A0A background.
- **Active States:** When a component is selected or "active," apply a **Glassmorphic** effect: a subtle background blur (8px) and a semi-transparent primary color overlay (10% opacity).
- **Glows:** Interactive elements (buttons, active toggles) use a `drop-shadow` with a 10px-15px blur in the primary or secondary color at low opacity (20-30%) to simulate the emission of light.

## Shapes

The shape language is **Soft (0.25rem)**. This provides a subtle modern touch without feeling "bubbly" or consumer-grade. The precision of the 90-degree corners is slightly eased to make the interface feel premium and high-end. 

- **Small elements (Checkboxes, Inputs):** 4px radius.
- **Large elements (Cards, Modals):** 8px or 12px radius.
- **Interactive Pill:** Use "Pill" shapes (rounded-full) specifically for play/stop controls and status badges.

## Components

- **Buttons:** 
  - *Primary:* Solid #00F2FF with black text. Apply a subtle cyan outer glow. 
  - *Ghost:* 1px border (#333) with White text. On hover, the border turns #00F2FF.
- **Progress Indicators:** Use linear gradients from #00F2FF to #39FF14. For audio meters, use a segmented "LED" style look where each block is separated by 1px of space.
- **Inputs:** Dark Slate (#1A1A1A) backgrounds with #333 borders. Focus state should trigger a #00F2FF border and a very subtle inner glow.
- **Cards:** Defined by #333 borders. Headers within cards should have a subtle bottom-border to separate title from content.
- **Chips/Badges:** Small, uppercase labels with a 10% opacity background of the primary or secondary color, matched with high-saturation text.
- **Tooltips:** Pure black (#000000) with a 1px #00F2FF border. Use for contextual help on complex synth parameters.
- **Knobs/Sliders:** While standard sliders are preferred for accessibility, visual representations should use the #00F2FF primary color for the "filled" track and #333 for the "empty" track.