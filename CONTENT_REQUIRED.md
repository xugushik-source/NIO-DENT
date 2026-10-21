# NIO DENT — Content Required

What is real on the demo, what is assumed, and what the clinic still has to send
before launch. ✅ confirmed source · ⚠️ taken from a public source but not yet
confirmed by the clinic · ❌ missing / illustrative

## Brand

| Item | Status | Notes |
|---|---|---|
| Name | ✅ | NIO DENT / ნიო-დენტი |
| Tagline | ✅ | "სტომატოლოგიისა და ესთეტიკის ცენტრი" — from their own Facebook banner |
| Logo | ⚠️ | Cut out of Facebook screenshots (`static/brand/`): pink flat logo for header/favicons, raspberry 3D lockup for the intro splash, white version for the footer. Need the original file (PNG/SVG) |
| Palette | ✅ | Blush white + raspberry from the logo, deep plum for buttons/footer (`static/css/tokens.css`) |

## Contact

| Item | Status | Notes |
|---|---|---|
| Phone | ✅ | +995 574 80 48 00 — dentos.ge and their posters |
| WhatsApp | ⚠️ | Assumed to be the same number — confirm |
| Email | ⚠️ | niodent.zugdidi@gmail.com — from dentos.ge |
| Address | ✅ | 58 M. Kostava St, Zugdidi; Google Maps link from dentos.ge |
| Hours | ⚠️ | 10:00–18:00 every day, as listed on dentos.ge — looks like a platform default, confirm |
| Facebook / Instagram | ✅ | facebook.com/dentistzugdidi, instagram.com/nio__dent |
| Payment methods | ⚠️ | Cash / card shown — confirm |

## Doctors (7, from dentos.ge)

| Doctor | Role | Photo |
|---|---|---|
| Maiko Khvichia | Therapist | ✅ from Facebook (birthday post) |
| Nino Ochigava | Therapist, surgeon, periodontist | ❌ "photo coming" card |
| Irakli Kezua | Prosthodontist | ❌ |
| Tamar Pachkoria | Oral & maxillofacial surgeon | ❌ |
| Tamar Chitanava | Therapist, surgeon | ❌ |
| Sopio Bigvava | Therapist, surgeon | ❌ |
| Nana Turdzeladze | Therapist | ❌ |

Bios are one factual sentence each. No experience years, education, certificates
or quotes are shown — none were invented. Languages show only Georgian until confirmed.
Nika Batiashvili (maxillofacial surgeon, visiting per a July poster) is **not** listed —
ask whether he should be.

## Services (12)

The directions listed on dentos.ge: therapy, implantology, prosthetics, surgery,
aesthetics, orthodontics, periodontology, endodontics, children's dentistry,
prevention/cleaning, X-ray diagnostics, consultation. **No prices are shown**
("price after consultation"). Real photos from the clinic's Facebook (20 April
seminar portraits, Irakli Kezua's smile poster, reception) are used on therapy, endodontics,
prosthetics, surgery, cleaning, periodontology, aesthetics and consultation; implants,
orthodontics, children's dentistry and X-ray still use generic illustrations. The people in
the seminar photos are not named anywhere — ask the clinic who is who.

## Technology

Only what the clinic claims itself: sterilisation ("the highest level, modern
equipment"), X-ray diagnostics (radiology), its own laboratory, a comfortable
setting. ELIT DENT's CBCT / microscope / intraoral-scanner claims were removed.

## Reviews

❌ 6 illustrative samples, labelled "Sample review" in the UI. No star rating is shown
(`site.json → rating.value` is null). Replace with real reviews (with consent).

## Before launch

1. Original logo, doctors' portraits, interior and treatment-room photos.
2. Confirm WhatsApp, hours, email, payment methods, doctors' languages.
3. Real reviews; then decide on a rating line.
4. Prices if they want them public.
5. Domain → `SITE_URL=https://… python3 build.py`, `featureFlags.demoMode: false`,
   clear `footer.disclosure` in all three `content/*.json`.
