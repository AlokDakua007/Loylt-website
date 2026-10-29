# LOYLT Website — HTML/CSS

A hand-coded HTML/CSS build of the **LOYLT Website → Home** frame from Figma (1440 × 7899).

## Run it

Open `index.html` in a browser, or serve the folder:

```bash
npx serve .        # or: python3 -m http.server
```

## Structure

```
index.html    page markup (one <section> per Figma section)
styles.css    all styles: design tokens, components, breakpoints
assets/       images (webp) and icons (svg) exported from Figma
fonts/        self-hosted Inter, Montserrat and DM Sans (woff2)
```

## Sections → classes

| Figma section | Class |
|---|---|
| Hero, nav and stats | `.hero`, `.nav`, `.hero__stats` |
| Trusted-by logo grid | `.trust`, `.logo-grid` |
| Services | `.services-wrap`, `.svc-grid` |
| Platform | `.platform`, `.feature-list` |
| Modules | `.modules`, `.mod-grid` |
| Loyalty programs | `.programs`, `.collage` |
| Rewards | `.rewards`, `.list-row` |
| UI/UX | `.uiux` |
| Industries and case studies | `.industries`, `.chips` |
| AI | `.ai` |
| Integrations and security | `.connect`, `.int-grid`, `.sec-grid` |
| Why LOYLT | `.why`, `.why-grid` |
| Results | `.results` |
| Testimonial | `.testi` |
| CTA | `.cta`, `.cta__card` |
| Footer | `.footer` |

## Design tokens

These live in `:root` in `styles.css`:

- **Colours:** `--blue`, `--teal`, `--teal-dark`, `--orange`, `--ice`, `--sky`
- **Layout:** `--rail` (1248px content width), `--gutter`

## Responsive behaviour

- **1440px and wider:** the layout matches the Figma frame pixel-for-pixel. Section offsets have been checked against Figma. Backgrounds fill the full width and the content stays on a centred 1248px rail.
- **≤1340px:** decorative images re-anchor to the right edge.
- **≤1100px:** the layout stacks into a tablet view and the nav links are hidden.
- **≤640px:** the layout becomes a single column for mobile.

## Fonts

The design uses **SF Pro Display**. It is used if it is installed locally. It is not bundled because of its licence. Otherwise the page falls back to Inter, size-adjusted to match SF Pro's metrics.
