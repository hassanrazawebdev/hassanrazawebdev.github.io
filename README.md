# Portfolio

Source for my portfolio site: **https://hassanrazawebdev.github.io**

I am a web designer and developer. I take sites from Figma layout to a live build, on my own,
end to end. Eight production sites so far across crypto, iGaming, music, ecommerce and construction.

## Why this repository looks the way it does

The site is one `index.html` file. That is deliberate, and it is part of what I am showing.

- **No framework.** Nothing to install, nothing to update, nothing that ships 90KB to render a page of text.
- **No web fonts.** System font stack, so the page needs exactly one network request: itself.
- **No build step.** What is in this repository is byte for byte what the browser receives.
- **Inline CSS and JS.** For a page this size, a separate stylesheet is a second round trip for no benefit.

Result: a single request, no render blocking assets, and the whole thing is readable top to bottom
by anyone reviewing it.

## What is in the page

| Part | What it demonstrates |
| --- | --- |
| Layout | CSS Grid with `auto-fill` and `minmax`, so the work grid reflows without a single media query breakpoint list |
| Type | Fluid scale using `clamp()`, no fixed pixel sizes |
| Theming | Design tokens as custom properties on `:root` |
| Motion | `IntersectionObserver` reveal, added only after the browser confirms support, and fully disabled under `prefers-reduced-motion` |
| Accessibility | Skip link, visible `:focus-visible` rings, semantic landmarks, real heading order, card links that expand to the whole card without nesting interactive elements |
| SEO | Canonical URL, Open Graph tags, and `Person` JSON-LD |
| Assets | Favicon is an inline SVG data URI, so there is no extra file and no extra request |

## Run it

There is no toolchain. Clone it and open the file.

```bash
git clone https://github.com/hassanrazawebdev/hassanrazawebdev.github.io.git
cd hassanrazawebdev.github.io
open index.html          # macOS
# or: start index.html   # Windows
# or serve it: python3 -m http.server 8000
```

## The work it links to

| Site | Sector | The interesting part |
| --- | --- | --- |
| [casinougc.com](https://casinougc.com/) | iGaming | Custom WordPress plugin powering the homepage front end where the page builder could not produce the layout |
| [electricalcalcs.online](https://electricalcalcs.online/) | Tools | 11 NEC referenced calculators, each showing its formula and the article it cites |
| [buildcalcpro.online](https://buildcalcpro.online/) | Construction | 15 material calculators with waste factor and regional rates as visible inputs |
| [musicclippingagency.com](https://musicclippingagency.com/) | Music | Animated data blocks, campaign results bubble chart, clip cohort diagram |
| [cryptoclippers.com](https://cryptoclippers.com/) | Crypto | Siloed vertical and platform page matrix routing into one booking funnel |
| [casinoclippingagency.com](https://casinoclippingagency.com/) | iGaming | Live metrics block and comparison pages built inside compliance constraints |
| [cryptougc.co](https://cryptougc.co/) | Web3 | Custom classed hero built on hand written CSS inside Elementor |
| [ecomugc.co](https://ecomugc.co/) | Ecommerce | Dual conversion path: booking widget plus contact form |

## Contact

- Email: hassanraza77450@gmail.com
- LinkedIn: [linkedin.com/in/hassanrazawebdesigner](https://www.linkedin.com/in/hassanrazawebdesigner/)

## License

MIT for the code. The site content, copy and project descriptions are mine.
