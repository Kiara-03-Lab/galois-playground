# Design System

A comprehensive design system for consistent, accessible, and maintainable interfaces.

## Color Tokens

### Base Colors
- **White**: `#FFFFFF` — primary background
- **Gray-100**: `#F5F5F5` — subtle backgrounds
- **Gray-300**: `#D1D5DB` — borders, dividers
- **Gray-500**: `#6B7280` — placeholder text
- **Gray-700**: `#374151` — secondary text
- **Gray-900**: `#111827` — primary text

### Brand Colors
- **Red**: `#DC2626` — primary CTA, errors, destructive actions
- **Orange**: `#F97316` — secondary CTA, highlights, badges
- **Green**: `#16A34A` — success states
- **Blue**: `#2563EB` — links, info states

## Color Hierarchy

Strategic use of color to create visual hierarchy and guide user attention:

- **White/Gray** → structure (80–90%)
  - Use neutral tones for the majority of the interface
  - Creates calm, professional appearance
  - Provides foundation for accent colors to stand out

- **Red** → action/danger (sparingly)
  - Reserved for critical actions and error states
  - Use minimally to maintain impact
  - Primary call-to-action color

- **Orange** → support/promotion
  - Secondary actions and highlights
  - Promotional elements and badges
  - Attention-getting but less critical than red

- **Green** → success/confirmation
  - Positive feedback and success states
  - Confirmation messages

- **Blue** → links/info
  - Hyperlinks and navigation
  - Informational states and messages

## Component States

### Interactive Element States
- **Default** → base color
- **Hover** → 10% darker or opacity shift
- **Active/Pressed** → 20% darker
- **Disabled** → Gray-300 background, Gray-500 text, no pointer events
- **Focus** → 2px ring, Blue or current color with offset

## Button Rules

### Button Variants
- **Primary CTA** → Red background, white text
- **Secondary CTA** → Orange background, white text
- **Tertiary** → Gray border, transparent background
- **Destructive** → Red outline or red background (context-dependent)

### Button Constraints
- **No red + orange buttons in same group**
  - Prevents visual competition
  - Maintains clear hierarchy

## Typography

### Font Family
- Primary: `'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', 'Helvetica Neue', sans-serif`
- Alternative: `'Noto Sans', -apple-system, BlinkMacSystemFont, 'Segoe UI', system-ui, sans-serif`

### Type Scale
- **H1**: `2rem` (32px) / bold
- **H2**: `1.5rem` (24px) / semibold
- **H3**: `1.25rem` (20px) / medium
- **Body**: `1rem` (16px) / regular / Gray-900
- **Secondary text**: `0.875rem` (14px) / Gray-700
- **Caption**: `0.75rem` (12px) / Gray-500

## Spacing Scale

Based on 4px base unit for consistent, harmonious spacing:

- **xs**: `4px`
- **sm**: `8px`
- **md**: `16px`
- **lg**: `24px`
- **xl**: `32px`
- **2xl**: `48px`

## Borders & Radius

### Border Properties
- **Border color**: Gray-300
- **Border width**: `1px` default

### Border Radius
- **sm**: `4px`
- **md**: `8px`
- **lg**: `12px`
- **full**: `9999px` (pill shape)

## Shadows/Elevation

Subtle shadows for depth and hierarchy:

- **sm**: `0 1px 2px rgba(0,0,0,0.05)`
- **md**: `0 4px 6px rgba(0,0,0,0.1)`
- **lg**: `0 10px 15px rgba(0,0,0,0.1)`

## Form Inputs

### Input States
- **Default** → Gray-300 border, white background
- **Focus** → Blue ring, Gray-900 text
- **Error** → Red border, Red text below
- **Success** → Green border (optional)
- **Placeholder** → Gray-500

## Links

### Link Styles
- **Default** → Blue, underline optional
- **Hover** → Blue darker, underline
- **Visited** → optional Purple or same as default

## Icons

### Icon Colors
- **Default** → Gray-700
- **Interactive** → inherit button/link color
- **Decorative** → Gray-500

## Accessibility

### Contrast Requirements
- **Normal text**: 4.5:1 minimum contrast ratio (text below 18pt or 14pt bold)
- **Large text/UI**: 3:1 minimum contrast ratio (18pt+ or 14pt+ bold text, UI components)

### Best Practices
- **Never use color alone for meaning** — always add text/icon
- **Focus visible** on all interactive elements
- **Test colorblind modes** (protanopia, deuteranopia)
- **Touch targets**: minimum 44×44px

## Dark Mode (if applicable)

### Color Adaptations
- **Background colors**: White `#FFFFFF` ↔ Gray-900 `#111827`
- **Text colors**: Gray-900 `#111827` ↔ White `#FFFFFF`
- **Borders**: Gray-300 `#D1D5DB` ↔ Gray-700 `#374151`
- **Red**: `#DC2626` ↔ `#EF4444` (lighter for dark backgrounds)
- **Orange**: `#F97316` ↔ `#FB923C` (lighter)
- **Green**: `#16A34A` ↔ `#22C55E` (lighter)
- **Blue**: `#2563EB` ↔ `#3B82F6` (lighter)
- **Shadows** ↔ reduced opacity or removed
- **Test contrast again** to ensure readability

## Hard Rules

Critical constraints to maintain design quality:

1. **No colored large backgrounds**
   - Keep large surfaces neutral
   - Use color strategically for accents

2. **No red + orange in same action group**
   - Prevents visual competition
   - Maintains clear hierarchy

3. **If everything pops, nothing matters**
   - Use restraint with accent colors
   - Let important elements stand out
