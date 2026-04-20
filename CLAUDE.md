# The Broad Strategy — Website

Luxury strategic advisory firm website. Single-page marketing site.

## Project Structure

```
broad/
  index.html            # Main site (single-page, all sections)
  privacy.html          # Privacy Policy
  terms.html            # Terms of Use
  css/
    v2.css              # Main stylesheet (tokens, layout, responsive)
    legal.css           # Styles for privacy/terms pages
  images/
    Broad-logo.png                   # Primary logo (nav + footer)
    Charleen-broad.png               # Founder photo (about section)
    Broad-video-Hero-trimmed.mp4     # Hero video (looping, trimmed)
```

## Brand Guidelines (strict)

- **Colors**: Crimson `#6D0504`, Gold `#C7A848`, Charcoal `#1C2026`, Off-white `#F8F6F2`
- **Fonts**: Playfair Display (headings), Lato (body text) — both via Google Fonts
- **Tone**: Luxury, refined, authoritative. No casual language.
- All design tokens live at the top of `css/v2.css` as CSS custom properties.

## Key Patterns

- **Scroll animations**: Elements with `.anim` classes are revealed via IntersectionObserver with staggered delays (`data-delay` attribute).
- **Nav**: Fixed top bar with scroll shadow (`scrolled` class). Mobile hamburger at <=640px.
- **Footer logo**: Uses `filter: brightness(0) invert(1)` to render white on dark background.
- **Pill buttons**: `border-radius: 100px` with SVG arrow icons (not HTML entities — avoids emoji rendering on iOS).
- **Section centering**: `.tag` and `.heading-lg` are centered by default. About section overrides to left-align within its card layout.

## Deployment

- **Live URL**: bonafidestudio.ca/broad/
- **FTP**: bonafidestudio.ca (port 21)
- **GitHub**: github.com/andrette07/broad
- No build tools or bundler — plain HTML/CSS/JS, open `index.html` directly.
- Hero video has zero side/bottom padding by design.
