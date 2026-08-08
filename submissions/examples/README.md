# CSS Morph-Glow Tooltip (Minimalist Tech Layout)

An intermediate, high-performance tooltip component built completely with pure CSS, tailored for Minimalist Tech and SaaS interfaces. Features a smooth shape morphing entrance combined with a soft atmospheric glow.

## 🚀 Features

- **Zero JavaScript:** Built entirely using pure CSS hover and focus states (`:hover`, `:focus-visible`) for fully responsive native tooltips.
- **Morphing Scale Entrance:** The tooltip element dynamically animates from `scale(0.9)`, a slight vertical offset, and a rounded bubble border radius into a crisp focus state (`scale(1)`, `border-radius: 8px`) using a performant `cubic-bezier(0.16, 1, 0.3, 1)` easing curve.
- **Minimalist Design:** Styled with delicate glassmorphism (`backdrop-filter: blur(16px)`), subtle borders, soft drop-shadows, and a refined blue atmospheric glow.
- **Accessible & Responsive:** Fully keyboard navigable via `focus-visible`. Includes fluid sizing for narrow screens and a strict `@media (prefers-reduced-motion: reduce)` override that neutralizes scale and morph transformations for sensitive users.

## 🛠️ Usage

Copy the HTML structure from `demo.html` and link the styles from `style.css`. Wrap any trigger element and its corresponding tooltip inside `.mt-tooltip-container`.

### CSS Custom Properties
Easily theme the component via the `:root` variables:

```css
:root {
    --mt-accent: #3b82f6;            /* Header code & glow color */
    --mt-speed: 0.35s;                /* Tooltip transition speed */
}
