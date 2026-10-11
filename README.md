# Resumio

Free, private, browser-only AI resume builder with an instant ATS score, smart job matching, company suggestions and writing tips. No account, no watermark, no uploads.

Built as a progressive enhancement on a single self-contained page. Your resume data never leaves your device; everything is analysed locally in your browser.

## Features

- Instant ATS score out of 100
- Smart job role and salary matching across 8 role families
- Company suggestions by industry and region
- Actionable resume writing tips
- Live resume strength meter
- Clean A4 PDF export (print based, ATS safe)
- Local auto-save with JSON import / export
- Mobile bottom sheets, dark theme and accent themes
- Accessible: skip link, ARIA labels, keyboard navigation

## Design

Resumio follows the design system in `assets/md/DESIGN.md`. The interface lives on a deep indigo canvas with an animated Blurple to magenta gradient mesh, using Blurple for primary actions, magenta for feature surfaces and electric green for the single high-intent action (Export PDF). Typography pairs Hanken Grotesk (display) with Plus Jakarta Sans (body).

## Project structure

```text
assets/
  img/           icons, favicons and the Open Graph image
  md/            DESIGN.md, SKILLS.md and brandcolours.css
index.html       the entire app: styles, markup and engine
manifest.webmanifest
robots.txt
sitemap.xml
404.html
```

## Run it locally

Just open `index.html` in a browser, or serve the folder on any static host:

```sh
python3 -m http.server 8080
```

Resumio is deployed at https://f9xr.org/resumio/.

## Privacy

Resumio is fully client side. It stores your resume in your browser's `localStorage` and never uploads it to a server. The analysis engine runs locally with no network requests.

## License

MIT. See LICENSE.