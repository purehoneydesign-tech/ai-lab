# Maria's Design System — Claude Reference

## Typography
- Font: Instrument Sans (Google Fonts)
- Display/headings: Instrument Sans 700–800, uppercase, tight tracking (-0.02em to -0.03em)
- Body: Instrument Sans 400, 15–16px, line-height 1.6–1.7
- Labels/meta: DM Mono 400, 10–11px, uppercase, letter-spacing 0.1em+
- No other fonts. Never Inter, Roboto, or system fonts.

## Colors
- Background: #0a0a0a (primary), #111111 (elevated), #1a1a1a (surface)
- Text: #f0f0f0 (primary), rgba(240,240,240,0.75) (secondary/subtext)
- Accent: #c8f060 (lime green) — use sparingly, never as background
- Borders: rgba(255,255,255,0.08) (default), rgba(255,255,255,0.15) (strong)

## Accessibility rules (always applied)
- Minimum contrast ratio: 4.5:1 for body text, 3:1 for large text
- Every interactive element needs :focus-visible styles
- No color as the only information carrier — always pair with text or shape
- Touch targets minimum 44x44px
- All images need alt text. All icon-only buttons need aria-label.

## Responsiveness
- Mobile-first. Base styles are mobile, desktop overrides in @media (min-width: 768px)
- Never use px for font sizes in media queries — use em
- Layouts: single column on mobile, grid on desktop
- Test at 375px (iPhone SE), 768px (tablet), 1280px (desktop)

## Component rules
- Border-radius: 2px for cells/tags, 4px for cards — never round unless intentional
- Transitions: 0.2s ease for hover states
- No box-shadows except for focus rings
- Spacing scale: 4, 8, 12, 16, 24, 32, 48px
