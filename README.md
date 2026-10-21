# NIO DENT

Demo website for **NIO DENT** — dental & aesthetic center in Zugdidi, Georgia
(58 M. Kostava St, +995 574 80 48 00). Georgian / English / Russian, Georgian by default.

Built on the ORDER PROFIT dental engine — the same pipeline, design system,
animations and booking/WhatsApp mechanics as ELIT DENT, with NIO DENT's own data,
logo, photos and a blush-white / raspberry palette taken from their logo.

**Status: demo for the clinic's review — not published.** See
`CONTENT_REQUIRED.md` for what is real vs. still missing and `NIO_BRIEF.md` for the
brief to send to the clinic.

## Build

```bash
pip install -r requirements-dev.txt
python3 build.py      # regenerates dist/
python3 validate.py   # must print "PASSED: 0 errors"
```

Preview locally: `cd dist && python3 -m http.server 8000`, then open
http://localhost:8000/ka/.

## Project layout

```
data/*.json          services, doctors, technology, reviews, site config (ka/en/ru)
content/{lang}.json  UI strings per language
templates/           Jinja2 templates
static/              CSS, JS, images, brand assets
build.py             the generator
validate.py          post-build checks
dist/                generated output — what gets deployed
docs/engine/         engine docs carried over from ELIT DENT (design audit,
                     replication contract, master build prompt)
```

## Where the content came from

- Clinic name, address, phone, email, map link, doctors and their specialties,
  "why NIO DENT" points, founding year (2010): niodent.dentos.ge.
- Logo and photos (Maiko Khvichia, reception with the gold logo wall, team photos):
  the clinic's public Facebook page (screenshots in the Drive folder "Nio denti"),
  cropped from screenshots — replace with originals from the clinic.
- Service photos: 8 of 12 from the clinic's Facebook; implants, orthodontics,
  children's dentistry and X-ray still use generic engine illustrations.
- Reviews: illustrative samples, labelled "Sample review" on every card.
