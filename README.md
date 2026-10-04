# Wascana Family Physiotherapy — website

A single-page marketing site for a **Regina, SK family physiotherapy clinic whose
specialty is women's health** (pelvic floor therapy, incontinence, pre/postnatal,
prolapse, pelvic pain, post-surgical recovery).

> ⚠️ **Demo content.** The clinic name, team bios, address, phone number, email and
> fee ranges are **fictional placeholders** (`555` phone block, `.example` email
> domain). Replace all of them — and the hero photo slot — before pointing a real
> audience at this site. Regulated-clinic advertising claims (fees, wait times,
> outcomes) must be verified against the real practice and the Saskatchewan
> College of Physical Therapists' guidelines.

## What's here

```
index.html              the site (self-contained HTML/CSS/JS; only external dep is Google Fonts)
designs/v1-generic.html first iteration — deliberately generic baseline
designs/critique.md     the design iteration: slop audit + Regina-fit critique + v2 decisions
```

## The design iteration

v1 was a competent-but-generic "women's wellness" page (violet gradients, centered
hero, icon-card grid, invented stats). It was then critiqued against **what actually
moves a Reginan patient**, and rebuilt as v2 (`index.html`). Key local-fit changes:

- **Direct access + coverage honesty up front** — in Saskatchewan you need *no
  referral* to see a physiotherapist, but Sask Health doesn't cover private visits;
  extended benefits (Blue Cross SK, Canada Life, Sun Life, Green Shield), WCB and
  SGI do. This is the first question local patients have, so it's in the hero trust
  strip and gets a whole section.
- **Phone-first conversion** — `(306)` call CTAs in the header, hero, and a sticky
  mobile call bar; the web form is secondary ("ask us to call you back").
- **Plain prairie voice** — the headline states the clinical bottom line
  ("Leaking when you laugh is common. It's also treatable.") instead of
  wellness-speak; the copy names the embarrassment barrier and de-mystifies the
  first visit, including consent-based internal assessment.
- **Local palette & type** — prairie paper/ink/terracotta/sage/wheat with one
  restrained dusty-rose accent (the prairie rose is Saskatchewan's provincial
  flower) instead of the "women's health = purple" cliché; Fraunces + Karla
  instead of default UI fonts.
- **Community texture** — drive-in communities (White City, Balgonie, Grand Coulee,
  Lumsden, Moose Jaw), winter-plowed parking, English/Punjabi/Hindi (Regina's real
  language mix), culturally safe care, and a Treaty 4 land acknowledgement.
- **The "family" half of the brief** — a family-physio strip so the whole
  household books, which is how these clinics actually fill chairs in a city of
  ~230k where everyone knows everyone.
- **Compliance hygiene** — invented stats and fake testimonials removed;
  transparency content (what to expect, fees, FAQ) replaces them.

## Run it

Open `index.html` in a browser, or serve locally:

```
python3 -m http.server 8080
```

## Live site

Published via GitHub Pages: **https://hermiona269.github.io/wascana-physio-web/**

## Suggested next steps

- Swap the hero photo slot for real clinic/team photography.
- Wire the call-back form to the clinic's booking system or email service.
- Add Google Business Profile + structured data (`LocalBusiness`/`MedicalClinic`).
- French language toggle (provincially useful in SK), if the team can staff it.
