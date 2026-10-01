---
name: Ledger Grid Protocol
colors:
  surface: '#f8f9ff'
  surface-dim: '#cbdbf5'
  surface-bright: '#f8f9ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#eff4ff'
  surface-container: '#e5eeff'
  surface-container-high: '#dce9ff'
  surface-container-highest: '#d3e4fe'
  on-surface: '#0b1c30'
  on-surface-variant: '#464554'
  inverse-surface: '#213145'
  inverse-on-surface: '#eaf1ff'
  outline: '#777586'
  outline-variant: '#c7c4d7'
  surface-tint: '#5148d7'
  primary: '#2a14b4'
  on-primary: '#ffffff'
  primary-container: '#4338ca'
  on-primary-container: '#c1beff'
  inverse-primary: '#c3c0ff'
  secondary: '#006a63'
  on-secondary: '#ffffff'
  secondary-container: '#99efe5'
  on-secondary-container: '#006f67'
  tertiary: '#5c2f00'
  on-tertiary: '#ffffff'
  tertiary-container: '#7d4200'
  on-tertiary-container: '#ffb477'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#e3dfff'
  primary-fixed-dim: '#c3c0ff'
  on-primary-fixed: '#100069'
  on-primary-fixed-variant: '#372abf'
  secondary-fixed: '#9cf2e8'
  secondary-fixed-dim: '#80d5cb'
  on-secondary-fixed: '#00201d'
  on-secondary-fixed-variant: '#00504a'
  tertiary-fixed: '#ffdcc3'
  tertiary-fixed-dim: '#ffb77d'
  on-tertiary-fixed: '#2f1500'
  on-tertiary-fixed-variant: '#6e3900'
  background: '#f8f9ff'
  on-background: '#0b1c30'
  surface-variant: '#d3e4fe'
typography:
  headline-lg:
    fontFamily: Geist
    fontSize: 1.75rem
    fontWeight: '600'
    lineHeight: 2.25rem
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Geist
    fontSize: 1.25rem
    fontWeight: '600'
    lineHeight: 1.75rem
    letterSpacing: -0.015em
  headline-sm:
    fontFamily: Geist
    fontSize: 1rem
    fontWeight: '600'
    lineHeight: 1.5rem
    letterSpacing: -0.01em
  body-lg:
    fontFamily: Geist
    fontSize: 0.875rem
    fontWeight: '400'
    lineHeight: 1.25rem
  body-md:
    fontFamily: Geist
    fontSize: 0.8125rem
    fontWeight: '400'
    lineHeight: 1.125rem
  body-sm:
    fontFamily: Geist
    fontSize: 0.75rem
    fontWeight: '400'
    lineHeight: 1rem
  mono-data-lg:
    fontFamily: JetBrains Mono
    fontSize: 0.875rem
    fontWeight: '500'
    lineHeight: 1.25rem
    letterSpacing: -0.02em
  mono-data-md:
    fontFamily: JetBrains Mono
    fontSize: 0.8125rem
    fontWeight: '500'
    lineHeight: 1.125rem
    letterSpacing: -0.01em
  mono-data-sm:
    fontFamily: JetBrains Mono
    fontSize: 0.75rem
    fontWeight: '400'
    lineHeight: 1rem
    letterSpacing: '0'
  label-caps:
    fontFamily: Geist
    fontSize: 0.6875rem
    fontWeight: '600'
    lineHeight: 0.875rem
    letterSpacing: 0.05em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  gutter: 0.75rem
  margin: 1rem
  space-xs: 0.125rem
  space-sm: 0.25rem
  space-md: 0.5rem
  space-lg: 0.75rem
  space-xl: 1rem
---

## Brand & Style
The design system embodies the precision of professional double-entry bookkeeping fused with the speed and kinetic polish of modern productivity engines like Linear and modern data workbenches. Built for operators managing daily physical and digital cash flows ("Registro diario de caja"), it removes visual clutter in favor of absolute legibility, spatial predictability, and data density.

The style is **Structured Modern-Technical**: crisp micro-borders, dense 28px–32px interactive rows, purposeful monospace numerical alignment, and subtle slate/indigo tones that ground high-stakes operations. The emotional tone is authoritative, error-proof, and calm under operational stress—delivering a fluid tactile sensation whether manipulated via mouse gestures or pure rapid keyboard navigation.

## Colors
The palette balances institutional trust with sharp tactical utility:
- **Primary (`#4338ca` - Deep Indigo)**: Drives focal interactions, selected active cells, active formula bars, and primary toolbar triggers.
- **Secondary (`#0f766e` - Deep Spruce / Teal)**: Used for positive cash inflows, balanced reconciliations, verified receipts, and locked settled transactions.
- **Tertiary (`#d97706` - Warm Amber)**: Flags pending adjustments, discrepancy warnings, cash drawer mismatch alerts, and unverified batch states.
- **Critical / Negative (`#dc2626` - Carmine)**: Reserved for cash outflows, negative balances, voided tickets, and hard validation breaks.
- **Neutral Palette (`#0f172a` to `#f8fafc`)**: Neutral slate foundation. Grid lines utilize `#e2e8f0` (subtle border) and `#cbd5e1` (structural partition), while alternating frozen and sticky panes layer between `#ffffff` and `#f8fafc`. Active focus outlines employ deep `#1e293b` with a 2px offset for rapid scanning.

## Typography
Typographic clarity defines the data surface:
- **Primary Text (`Geist`)**: Used across toolbar actions, column headers, system dialogs, and text descriptors (e.g., transaction reasons, supplier names).
- **Monospace Data (`JetBrains Mono`)**: Strict requirement for all currency figures, timestamps, ledger balances, receipt IDs, and decimal multipliers. Guarantees character width uniformity down every column, preventing optical jitter during rapid vertical scanning.
- **Alignment Rules**: All numerical/currency entries must be aligned right with `mono-data-*`. Textual descriptions align left with `body-*`. Status tags and operation codes align center. All uppercase labels (`label-caps`) use explicit positive letter spacing for legibility at small sizes.

## Layout & Spacing
The layout implements a high-density, viewport-filling fixed-canvas system:
- **Canvas Shell**: Top toolbar (height: 48px), secondary filter & summary band (height: 40px), grid container (fills remaining vertical height with internal dual-axis scroll), and persistent bottom status reconciliation footer (height: 36px).
- **Cell Proportions**: Standard rows default to a strict 32px height, with an optional compact view at 26px. Horizontal cell padding is pinned to `space-md` (8px) on data columns and `space-lg` (12px) on column headers.
- **Breakpoints**: 
  - **Desktop (>= 1280px)**: Multi-column side drawer for detailed split receipts, full pinned summary bar, visible column reordering handles.
  - **Laptop/Tablet Landscape (768px - 1279px)**: Side drawers convert to overlay sheets; secondary metadata columns automatically collapse behind a toggleable column manager; toolbar actions collapse into icon dropdowns.
  - **Mobile (< 768px)**: The infinite sheet transitions into single-entry verification cards with a pinned horizontal sticky subtotal bar; full grid horizontal scroll locked with first column (ID/Time) sticky.

## Elevation & Depth
This system eliminates heavy, atmospheric drop shadows in favor of **structural boundaries and planar stacking**:
- **Layer 0 (Canvas Base)**: The foundational table surface (`#ffffff`) with 1px `#e2e8f0` grid borders.
- **Layer 1 (Sticky Elements & Freezes)**: Sticky header rows and left-pinned ledger columns use high-opacity solid backgrounds (`#f8fafc`) paired with a 1px solid border (`#cbd5e1`) and a directional micro-edge (`box-shadow: 0 1px 2px rgba(15, 23, 42, 0.06)` for horizontal sticky columns).
- **Layer 2 (Popovers, Context Menus & Tooltips)**: Strict 1px `#cbd5e1` outline with a precise ambient elevation (`0 4px 12px -2px rgba(15, 23, 42, 0.08), 0 2px 4px -1px rgba(15, 23, 42, 0.04)`).
- **Active Selection**: Focused cells and multi-cell bounding boxes project zero blur, relying entirely on a sharp 2px solid `#4338ca` ring with an inner 1px white contrast spacer.

## Shapes
To maximize data density and mimic physical bookkeeping machinery, elements employ minimal rounding (`0.25rem` / 4px base):
- Grid cells maintain perfectly square inner corners (0px) to prevent optical gaps and inconsistent grid intersections.
- Interactive controls (inputs, dropdown triggers, toolbar buttons) use `0.25rem` radii.
- Status chips and badges utilize slightly softer pill or 4px contours, maintaining compact structural boundaries.
- Modals, flyout sheets, and floating filter cards use `0.375rem` (6px) outer corners to communicate distinct layering without sacrificing technical rigor.

## Components

### Grid Cell & Input Behavior
- **Default State**: Transparent background, border-right and border-bottom 1px solid `#e2e8f0`. High contrast `#0f172a` text.
- **Editing State**: Cell background becomes `#ffffff`. Surrounding border is overtaken by a 2px `#4338ca` outline extending 1px beyond the cell edge. Monospace numerical input fields fill 100% of cell area without native browser chrome.
- **Locked / Read-Only**: Shaded with `#f8fafc`, text color subdued to `#64748b`, displaying an inline subtle padlock icon on hover.

### Status Badges
- **Locked/Settled Row**: Background `#f0fdf4`, border `#bbf7d0`, text `#15803d` with monospace lock glyph (`LKD`).
- **Editable/Draft Row**: Background `#f8fafc`, border `#e2e8f0`, text `#475569` (`OPEN`).
- **Discrepancy/Review**: Background `#fffbeb`, border `#fde68a`, text `#b45309` (`REV`).
- Badges measure 18px in total height, using `label-caps` font, padding 0 6px.

### Toolbar & Action Rail
- Houses quick-action triggers: "Nuevo Movimiento" (Primary button, solid `#4338ca`, white text), "Cerrar Caja" (Secondary teal button), and icon-accompanied utility triggers: "Importar extracto" (.csv/XLSX) and "Exportar" (PDF/Excel dropdown).
- Integrates a real-time ledger status indicator: total income, total expense, and net daily balance prominently displayed with colored mini-metrics.

### Form & Filter Inputs
- Inputs feature a crisp 1px solid `#cbd5e1` resting state, transitioning to `#4338ca` on focus with no diffuse glow.
- Quick search filters operate with zero latency, highlighting matching rows dynamically.

### Sticky Headers & Summary Footer
- **Column Headers**: Height 32px, text transformed to uppercase using `label-caps` with subtle sort indicators and column-resize dividers. Background `#f1f5f9`.
- **Reconciliation Footer**: Sticky to viewport bottom, displaying live column sums (Debit, Credit, Difference) strictly aligned under their respective parent columns in `mono-data-md` bold.