# MetricAscent OS — Prospect Demo

The interactive prototype of MetricAscent OS, shown to prospective clients.

Live at **[revenue.metricascent.com](https://revenue.metricascent.com)** (GitHub Pages, published from `main`).

It walks a prospect through a working revenue-operations command centre for an
independent window & door company, using **Summit Windows & Doors** — a fictional
reference company — as the worked example. Every figure on screen is illustrative
demo data for Summit, not a client's real numbers.

## What it demonstrates

Mission Control, plus the connected modules a prospect sees on the tour: lead
capture and qualification, messaging, follow-up, scheduling, quoting, financing,
rebates and incentives, measurement verification, order status, schedule
optimisation, reviews, reactivation, and content.

## Structure

- `index.html` — the entire prototype: one self-contained file, inline CSS and JS,
  views rendered client-side. This is what the domain serves.
- `metricascent-os.html` — a byte-identical copy of `index.html`, kept so the
  prototype can also be linked under that name. **Edit both together, or they
  drift apart.**
- `CNAME` — pins the custom domain.
- `assets/`, `favicon.ico` — images from the earlier marketing site. The prototype
  does **not** reference `assets/`; only `favicon.ico` is used.
- `metricascent-site.zip` — archived copy of the earlier marketing site, kept
  deliberately. Note it is publicly downloadable from the live domain.

The only runtime dependency is **Google Fonts (Inter)**. Icons are inline SVG, so
the prototype renders offline apart from the font.

## Run locally

Open `index.html` in a browser, or serve the folder:

```bash
python -m http.server 8000
```

Then visit http://localhost:8000.

## Claims shown to prospects

Anything on screen that asserts a fact about the industry or about law — as
opposed to Summit's illustrative demo numbers — must trace to a primary source,
name the population it measures, and be re-checked before a demo.

Marketing aggregators routinely restate figures with the number or the population
altered and the citation dropped; several such claims have already been removed
from this prototype. Where no credible benchmark exists for window & door
specifically, the prototype says so rather than borrowing a cross-industry figure.

Legal and tax facts age. The federal §25C energy credit ended for property placed
in service after 31 December 2025, and the prototype reflects that.
