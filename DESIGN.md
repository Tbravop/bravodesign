---
name: Ethical Neo-Memphis
colors:
  surface: '#fcf9f8'
  surface-dim: '#dcd9d9'
  surface-bright: '#fcf9f8'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f6f3f2'
  surface-container: '#f0eded'
  surface-container-high: '#eae7e7'
  surface-container-highest: '#e5e2e1'
  on-surface: '#1c1b1b'
  on-surface-variant: '#464650'
  inverse-surface: '#313030'
  inverse-on-surface: '#f3f0ef'
  outline: '#777681'
  outline-variant: '#c7c5d1'
  surface-tint: '#56589a'
  primary: '#56589a'
  on-primary: '#ffffff'
  primary-container: '#9a9ce4'
  on-primary-container: '#2f3172'
  inverse-primary: '#c0c1ff'
  secondary: '#5e5e5d'
  on-secondary: '#ffffff'
  secondary-container: '#e0dfde'
  on-secondary-container: '#626361'
  tertiary: '#5e5e5e'
  on-tertiary: '#ffffff'
  tertiary-container: '#a2a2a2'
  on-tertiary-container: '#383838'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#e1e0ff'
  primary-fixed-dim: '#c0c1ff'
  on-primary-fixed: '#101054'
  on-primary-fixed-variant: '#3e4081'
  secondary-fixed: '#e3e2e0'
  secondary-fixed-dim: '#c7c6c5'
  on-secondary-fixed: '#1a1c1b'
  on-secondary-fixed-variant: '#464746'
  tertiary-fixed: '#e2e2e2'
  tertiary-fixed-dim: '#c6c6c6'
  on-tertiary-fixed: '#1b1b1b'
  on-tertiary-fixed-variant: '#474747'
  background: '#fcf9f8'
  on-background: '#1c1b1b'
  surface-variant: '#e5e2e1'
typography:
  display:
    fontFamily: system-ui
    fontSize: 72px
    fontWeight: '900'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: system-ui
    fontSize: 48px
    fontWeight: '800'
    lineHeight: '1.2'
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: system-ui
    fontSize: 32px
    fontWeight: '800'
    lineHeight: '1.2'
  headline-md:
    fontFamily: system-ui
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.3'
  body-lg:
    fontFamily: system-ui
    fontSize: 20px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: system-ui
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-mono:
    fontFamily: monospace
    fontSize: 14px
    fontWeight: '600'
    lineHeight: '1'
spacing:
  base: 8px
  xs: 4px
  sm: 12px
  md: 24px
  lg: 48px
  xl: 80px
  border-width: 4px
  shadow-offset: 6px
---

## Brand & Style
The design system adopts an **Ethical Neo-Brutalist** aesthetic fused with **Memphis Group** geometry. It prioritizes digital sustainability and performance through zero-asset typography and lightweight CSS-driven patterns. The brand personality is unapologetically honest, structurally transparent, and highly accessible. It avoids the "dark patterns" of modern soft UI in favor of high-contrast, high-legibility components that respect user agency and hardware constraints.

The visual narrative is defined by:
- **Raw Structural Integrity:** Heavy strokes and hard shadows that make the interface's hierarchy physical and undeniable.
- **Memphis Playfulness:** Use of geometric primitives (dots, grids, and zig-zags) to break the rigidity of standard layouts.
- **Ethical Performance:** Leveraging system-native stacks to ensure the fastest possible time-to-interactive while maintaining a bespoke, designerly feel.

## Colors
The palette is built on high-contrast foundations to exceed WCAG AA and AAA accessibility standards.

- **Primary (Lavender #9A9CE4):** Used for interactive elements, focus states, and primary actions. It provides a soft visual counterpoint to the aggressive black strokes.
- **Surface (Bone #F9F8F6):** A warm, off-white background that reduces eye strain compared to pure white, serving as the canvas for all components.
- **Accents (Pure Black #000000):** Used for all borders (4px), hard shadows, and typography.
- **Functional States:** Success, Error, and Warning states should use high-saturation variants of Green, Red, and Yellow, always encased in 4px black borders to maintain stylistic consistency.

## Typography
This design system utilizes the **System Font Stack** to eliminate HTTP requests and prioritize performance. 

- **Headlines:** Use `system-ui` (San Francisco on iOS/Mac, Segoe UI on Windows, Roboto on Android) with heavy weights (800-900) for a bold, editorial feel.
- **Body:** Standard `system-ui` at weight 400 for maximum legibility across all platforms.
- **Labels/Data:** A monospaced font stack (SFMono, Consolas, or Liberation Mono) is used for metadata, buttons, and small labels to reinforce the technical/brutalist aesthetic.

## Layout & Spacing
The layout follows a **Fixed-Fluid Hybrid** model. Content is contained within a 12-column grid on desktop (max-width: 1280px) and collapses to a single column on mobile.

- **The Grid:** Use 24px gutters. Elements should align strictly to the grid lines. 
- **The "Bento" Logic:** Layouts should be composed of distinct, bordered boxes.
- **Patterns:** Empty space should occasionally be filled with CSS-generated patterns:
  - **Dot Matrix:** `background-image: radial-gradient(#000 1px, transparent 0); background-size: 20px 20px;`
  - **Grid:** 40px square grid using thin 1px lines as a background texture behind 4px-bordered components.

## Elevation & Depth
Depth is strictly two-dimensional and physical. There are no soft shadows or blurs.

- **Hard Shadows:** Use a solid black box-shadow offset to the bottom-right. The offset is typically `6px 6px 0px 0px #000`.
- **Interaction Depth:** When an element (like a button) is pressed, the shadow offset reduces to `2px 2px`, and the element translates `4px` down and right, simulating a physical "click."
- **Layering:** Hierarchy is established by z-index stacking. A "higher" element does not get a larger blur; it simply sits further "out" from its shadow anchor.

## Shapes
The design system uses a **Sharp (0px)** roundedness philosophy. Every container, button, and input must have perfectly square corners. This reinforces the brutalist nature of the design.

Geometric accents (circles or triangles) may be used for decorative icons or patterns, but functional UI containers must remain strictly rectangular. All strokes are consistent at 4px.

## Components
Consistent implementation of components ensures the Neo-Brutalist integrity of the design system.

- **Buttons:** 4px black border, Lavender (#9A9CE4) background, and a 6px hard black shadow. Text is bold and monospaced. On hover, the background color can shift to a brighter highlight.
- **Input Fields:** Bone (#F9F8F6) background with a 4px black border. Focus state changes the border color to Lavender or increases the thickness of the hard shadow.
- **Cards:** Defined by a 4px black border. Every card must have a hard shadow. Headers within cards should be separated by a 4px horizontal rule.
- **Lists:** Items are separated by 4px black lines. Selected items use the Lavender background.
- **Checkboxes & Radios:** Large, 24px squares or circles with 4px borders. The "checked" state is a solid black fill or a large "X" for checkboxes.
- **Geometric Accents:** Use SVG-based crosses (x) and pluses (+) as bullet points or decorative corner ornaments to lean into the Memphis style.