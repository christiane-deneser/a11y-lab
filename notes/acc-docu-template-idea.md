# Accessible Button Component

## Purpose

A semantic `<button>` element with clear focus states and robust behavior.
This component is the base for interactive controls in a design system.

It supports:
- Keyboard-only users
- Screen reader users
- Users with attention / focus challenges (clear affordances and feedback)

## Variants

- **Primary** – main call to action
- **Secondary** – less prominent action
- **Disabled** – non-interactive, clearly communicated state

## Accessibility Notes

- Uses native `<button>` element (no `div` with click handlers)
- Focusable via `Tab`
- Activates with `Enter` and `Space`
- Visible focus outline (not removed)
- Sufficient color contrast between:
  - text and background
  - button and surrounding content
- No ARIA needed for basic buttons

### Cognitive / Neuro-Inclusive Notes

- Clear label text (no vague “Click here”)
- Avoids multiple high-importance buttons in one view
- Consistent placement across pages
- Uses size/weight hierarchy instead of only color to signal importance

## Code Example

See [`index.html`](./index.html) and [`styles.css`](./styles.css)  
for the complete HTML/CSS implementation.

```html
<button class="btn btn-primary">
  Save changes
</button>
```

## Testing
* Keyboard: Tab, Shift+Tab, Enter, Space
* Screen readers: NVDA, VoiceOver, or TalkBack basic announcement
* Automated: axe, Accessibility Insights, Lighthouse

## References
* WCAG 2.2 – 2.1 Keyboard Accessible, 2.4.7 Focus Visible
* ARIA Authoring Practices – Button Pattern

