---
name: Vibrant Portfolio System
colors:
  surface: '#faf8ff'
  surface-dim: '#d8d9e6'
  surface-bright: '#faf8ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f2f3ff'
  surface-container: '#ecedfa'
  surface-container-high: '#e7e7f4'
  surface-container-highest: '#e1e2ee'
  on-surface: '#191b24'
  on-surface-variant: '#424656'
  inverse-surface: '#2e303a'
  inverse-on-surface: '#eff0fd'
  outline: '#737687'
  outline-variant: '#c2c6d9'
  surface-tint: '#0053da'
  primary: '#004cca'
  on-primary: '#ffffff'
  primary-container: '#0062ff'
  on-primary-container: '#f3f3ff'
  inverse-primary: '#b4c5ff'
  secondary: '#006c49'
  on-secondary: '#ffffff'
  secondary-container: '#6cf8bb'
  on-secondary-container: '#00714d'
  tertiary: '#9e3100'
  on-tertiary: '#ffffff'
  tertiary-container: '#c84000'
  on-tertiary-container: '#fff1ed'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#dbe1ff'
  primary-fixed-dim: '#b4c5ff'
  on-primary-fixed: '#00174b'
  on-primary-fixed-variant: '#003ea8'
  secondary-fixed: '#6ffbbe'
  secondary-fixed-dim: '#4edea3'
  on-secondary-fixed: '#002113'
  on-secondary-fixed-variant: '#005236'
  tertiary-fixed: '#ffdbcf'
  tertiary-fixed-dim: '#ffb59c'
  on-tertiary-fixed: '#390c00'
  on-tertiary-fixed-variant: '#832700'
  background: '#faf8ff'
  on-background: '#191b24'
  surface-variant: '#e1e2ee'
typography:
  headline-xl:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '800'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-caps:
    fontFamily: geist
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1'
    letterSpacing: 0.05em
  code:
    fontFamily: geist
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.5'
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 8px
  container-max: 1200px
  gutter: 24px
  margin-mobile: 20px
  margin-desktop: 64px
---

## Brand & Style

The design system is built on a foundation of **Modern Minimalism** with an **Energetic Professional** edge. It is designed specifically for developer portfolios where clarity of code and technical expertise must meet high-end aesthetic execution. 

The personality is "Airy yet Precise." By utilizing expansive whitespace and a high-energy primary accent, the UI feels breathable and optimistic. The design style avoids heavy shadows or complex gradients, opting instead for a flat, crisp architecture that prioritizes content legibility and professional rigor. It balances the "high-tech" feel of software engineering with the "high-touch" feel of modern digital design agencies.

## Colors

The palette is anchored by a vibrant "Electric Blue" primary color used sparingly for high-impact actions and brand markers. The background system relies on a stark white base for core content and a subtle "Cool Grey" for structural differentiation.

- **Primary:** An energetic blue used for CTA buttons, active states, and focus indicators.
- **Secondary:** A fresh emerald green utilized for success states and secondary highlights.
- **Surface System:** Pure white (#FFFFFF) for cards and primary content containers, set against a light-grey (#F8FAFC) global background to create a soft "layered" effect without relying on shadows.
- **Contrast:** High-contrast text (#0F172A) ensures maximum readability for technical documentation and project descriptions.

## Typography

The typography system uses **Inter** for its incredible versatility and readability in digital interfaces. To lean into the "developer" aspect of the portfolio, **Geist** is introduced for labels and code snippets to provide a technical, monospaced-adjacent aesthetic.

- **Headlines:** Use tight tracking and heavy weights to create a strong visual hierarchy.
- **Body:** Generous line-height (1.6) is mandatory to maintain the "airy" feel.
- **Labels:** Small caps and increased letter spacing are used for metadata like dates, categories, or tech-stack tags.
- **Mobile scaling:** For devices below 768px, `headline-xl` should scale down to 36px to prevent awkward line breaks.

## Layout & Spacing

This design system employs a **Fixed Grid** philosophy for desktop to maintain a premium, editorial feel, transitioning to a fluid system for mobile devices.

- **Grid:** A 12-column grid with a 24px gutter.
- **Rhythm:** All spacing is derived from a base unit of 8px. Use 16px, 32px, 64px, and 128px increments for vertical section spacing to ensure a high-airflow layout.
- **Margins:** Desktop views should feature wide horizontal margins (64px+) to keep content centered and focused.
- **Stacking:** Elements like project cards should use a 32px vertical gap to allow each piece of work to breathe independently.

## Elevation & Depth

To maintain a minimalist and clean aesthetic, this design system avoids heavy shadows. Instead, it uses **Tonal Layering** and **Low-Contrast Outlines**.

- **Surfaces:** Use #FFFFFF for components placed on the #F8FAFC background.
- **Outlines:** Instead of shadows, use a 1px border (#E2E8F0) to define container edges.
- **Interactive Depth:** On hover, a subtle, highly diffused shadow (0px 10px 20px rgba(0, 0, 0, 0.04)) can be applied to cards to signal interactivity without breaking the flat aesthetic.
- **Focus States:** Use a 2px solid primary color ring with a 2px offset to maintain accessibility and energetic feedback.

## Shapes

The shape language is "Soft-Modern." We use a consistent, tight radius to keep the UI feeling organized and professional rather than playful or bubbly.

- **Primary Radius:** 6px (Standard for buttons, inputs, and small cards).
- **Large Radius:** 12px (Used for large project containers or modal windows).
- **Interactive Elements:** Maintain the same radius for focus states and selections to ensure visual continuity.

## Components

- **Buttons:** Solid primary color for main actions. Ghost buttons (transparent background with a 1px border) for secondary actions. Use `label-caps` for button text to enhance the professional feel.
- **Project Cards:** Pure white backgrounds with 1px border. Feature high-quality imagery with a 0px top-radius if the image is flush, or 6px if contained.
- **Tech Chips:** Small, light grey backgrounds (#F1F5F9) with `body-sm` text. Use no border.
- **Inputs:** Clean white fields with a #E2E8F0 border. On focus, the border transitions to the primary color.
- **Status Indicators:** Use the secondary emerald green for "Available for Work" badges to provide a fresh, positive signal.
- **Code Blocks:** Utilize a slightly darker neutral (#1E293B) for code blocks to provide a "dark mode" anchor for technical content within the light UI.