---
name: Lumina Soft-Precision
colors:
  surface: '#f7f9fb'
  surface-dim: '#d8dadc'
  surface-bright: '#f7f9fb'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f2f4f6'
  surface-container: '#eceef0'
  surface-container-high: '#e6e8ea'
  surface-container-highest: '#e0e3e5'
  on-surface: '#191c1e'
  on-surface-variant: '#45464d'
  inverse-surface: '#2d3133'
  inverse-on-surface: '#eff1f3'
  outline: '#76777d'
  outline-variant: '#c6c6cd'
  surface-tint: '#565e74'
  primary: '#000000'
  on-primary: '#ffffff'
  primary-container: '#131b2e'
  on-primary-container: '#7c839b'
  inverse-primary: '#bec6e0'
  secondary: '#00668a'
  on-secondary: '#ffffff'
  secondary-container: '#40c2fd'
  on-secondary-container: '#004d6a'
  tertiary: '#000000'
  on-tertiary: '#ffffff'
  tertiary-container: '#271901'
  on-tertiary-container: '#98805d'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#dae2fd'
  primary-fixed-dim: '#bec6e0'
  on-primary-fixed: '#131b2e'
  on-primary-fixed-variant: '#3f465c'
  secondary-fixed: '#c4e7ff'
  secondary-fixed-dim: '#7bd0ff'
  on-secondary-fixed: '#001e2c'
  on-secondary-fixed-variant: '#004c69'
  tertiary-fixed: '#fcdeb5'
  tertiary-fixed-dim: '#dec29a'
  on-tertiary-fixed: '#271901'
  on-tertiary-fixed-variant: '#574425'
  background: '#f7f9fb'
  on-background: '#191c1e'
  surface-variant: '#e0e3e5'
typography:
  headline-xl:
    fontFamily: Hanken Grotesk
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-xl-mobile:
    fontFamily: Hanken Grotesk
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Hanken Grotesk
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Hanken Grotesk
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
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
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  label-md:
    fontFamily: Geist
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 16px
    letterSpacing: 0.02em
  label-sm:
    fontFamily: Geist
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 14px
    letterSpacing: 0.04em
rounded:
  sm: 0.5rem
  DEFAULT: 1rem
  md: 1.5rem
  lg: 2rem
  xl: 3rem
  full: 9999px
spacing:
  base: 8px
  xs: 4px
  sm: 12px
  md: 24px
  lg: 48px
  xl: 80px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 48px
---

## Brand & Style
This design system balances high-performance utility with an approachable, organic aesthetic. It targets professional environments that prioritize efficiency but wish to avoid the sterile coldness of traditional enterprise software. 

The style is **Modern Corporate with a Tactile Softness**, blending the rigorous clarity of a systematic grid with hyper-rounded geometry. The emotional response should be one of "effortless precision"—software that feels advanced and powerful, yet safe and inviting to interact with. High-quality whitespace and refined typography ensure that the extreme roundedness feels intentional and sophisticated rather than juvenile.

## Colors
The palette is rooted in deep slate and vibrant sky tones to maintain a professional, tech-forward energy.

- **Primary**: A deep, authoritative Navy Slate used for primary actions and text hierarchy.
- **Secondary**: A bright, energetic Sky Blue used for accents, active states, and highlights.
- **Neutral**: A range of cool grays (Slate) used for backgrounds, borders, and subtle containment.
- **Surface**: Pure white is used for card backgrounds to maximize contrast against the soft neutral page background.

## Typography
The typography system uses a tri-font approach to differentiate intent:
- **Headlines**: Hanken Grotesk provides a sharp, contemporary edge that contrasts beautifully with the rounded UI shapes.
- **Body**: Inter ensures maximum readability for long-form content and data.
- **Labels/Technical**: Geist (monospaced-leaning) is used for small labels, buttons, and data points to reinforce the "Precision" aspect of the system.

## Layout & Spacing
The system utilizes a **12-column Fluid Grid** for desktop and a **4-column Fluid Grid** for mobile. 

Spacing follows a strict 8px base unit. To complement the maximum roundedness of the components, internal padding in containers should be generous (typically `md` or 24px) to prevent content from getting "clipped" by the deep corner radii. 

On mobile, margins are reduced to 16px, but the gutter remains 24px to ensure distinct separation between highly rounded elements.

## Elevation & Depth
Depth is achieved through **Tonal Layers** supplemented by **Ambient Shadows**. 

1.  **Level 0 (Background)**: The base neutral color.
2.  **Level 1 (Cards/Containers)**: White surfaces with a very soft, diffused shadow (0px 4px 20px rgba(0,0,0,0.05)).
3.  **Level 2 (Overlays/Popovers)**: Elevated surfaces with a more pronounced shadow (0px 10px 30px rgba(0,0,0,0.08)).

Avoid harsh borders; instead, use 1px subtle strokes in a slightly darker neutral shade only when elements sit on a background of the same color.

## Shapes
This design system utilizes **maximum roundedness** to create a soft, modern, and friendly interface. 

- **Components**: All small to medium components (Buttons, Inputs, Chips) are **Pill-shaped**, meaning the border-radius is essentially half of the height or set to a minimum of 999px.
- **Containers**: Larger elements like Cards, Modals, and Sidebars use a consistent **24px to 32px radius** (`rounded-xl` to `rounded-2xl`).
- **Nesting**: When nesting rounded elements, ensure the inner element's radius is smaller than the outer element's radius to maintain visual harmony.

## Components
- **Buttons**: Fully pill-shaped (rounded-full). Height should be 40px or 48px. Use Geist for button text in uppercase or medium weight for a technical feel.
- **Inputs**: Fully pill-shaped. Maintain a minimum height of 48px. Left-align text with generous 20px horizontal padding to clear the curve.
- **Chips**: Small, pill-shaped badges used for tagging and status. Use a subtle background tint of the primary or secondary color.
- **Cards**: Use 24px corner radius. Content inside should be inset by at least 24px to ensure it doesn't collide with the deep corners.
- **Lists**: List items should have rounded corners (12px) when hovered or selected, creating a "floating" feel within the list container.
- **Checkboxes & Radios**: Checkboxes use a 4px radius (softened), while Radio buttons remain perfect circles to match the pill-based language.