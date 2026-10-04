# Design Iteration — v1 → v2 (Regina fit)

**Brief:** website for a Regina family physiotherapy clinic whose specialty is women's health.
**Method:** build a competent generic draft (v1), critique it against (a) an anti-slop audit and (b) what actually moves a Reginan patient, then rebuild (v2 = `../index.html`).

---

## 1. Slop diagnostic of v1 — 7/10

| # | Tell | Fires? | Evidence in v1 |
|---|------|--------|----------------|
| 1 | Tech gradient | ✗ | violet gradients on h1, buttons, CTA band |
| 2 | Generic tech hue | ✗ | indigo/violet accent — plus the "women's health = purple/pink" cliché |
| 3 | Feature-tile grid | ✗ | six equal-weight icon cards, nothing prioritized |
| 4 | Accent rail | ✓ | — |
| 5 | Unearned blur | ✓ | — |
| 6 | Monument stat | ✗ | invented "12+ / 2,500+ / 98%" — unverified claims a regulated clinic can't make |
| 7 | Icon topper | ✗ | rounded-square emoji above every card heading |
| 8 | Center stack | ✗ | every section centered; no real composition |
| 9 | Default type | ✗ | Inter/system-ui |
| 10 | Wrong surface | ✓ | Decide/Learn is right for a clinic site |

Also: the emoji logo renders as tofu boxes (□) on systems without an emoji font — confirmed in the v1 screenshot.

## 2. Regina-fit critique — what v1 gets wrong *for this audience*

1. **Zero practical-access info.** In Saskatchewan: no physician referral is required to see a physiotherapist (direct access), but Saskatchewan Health does **not** cover private clinic visits — most people pay via extended health benefits (Blue Cross SK, Canada Life, Sun Life, Green Shield…), WCB, or SGI. For a city with a large public-sector workforce and median household income ~$88k, "do I need a referral / will my insurance cover it / what does it cost" is the *first* question. v1 answers none of them.
2. **Booking model mismatch.** v1's only conversion path is a web form. Prairie clinics run on the phone; a Regina patient wants a `306` number and a human. Phone must be the primary CTA (and a sticky call button on mobile).
3. **Tone is big-city spa.** "Reclaim confidence… your unique journey" reads as fluff to a prairie audience that trusts plain talk. The headline should say the most important clinical thing in the plainest words: leaking when you laugh/cough/sneeze is common and treatable.
4. **Nothing says Regina.** No neighbourhood or drive-in communities (White City/Emerald Park, Balgonie, Grand Coulee, Lumsden, Moose Jaw), no winter/parking reality (−30°C mornings and a plowed lot are a genuine booking factor), no mention of languages (Regina's clinics commonly serve English, Punjabi, Hindi, and more; ~10% of the city is Indigenous — culturally safe, judgment-free care must be *stated*, not implied), no Treaty 4 land acknowledgement (standard for SK health organizations).
5. **The embarrassment barrier is underworked.** For pelvic health, shame is the #1 reason women wait years. v1 mentions it once in a decorative band. v2 should lead with it and de-mystify the first visit (internal exam is consent-based and optional at each step — the question everyone is afraid to ask).
6. **The "family" half of the brief is missing.** It's a *family* physio clinic with a women's-health specialty. In Regina, multi-gen families book together — grandma's balance, teenager's sprain, new mom's recovery. One strip covering general family physio turns the specialty clinic into a whole-family option (and that's the referral engine).
7. **Fake testimonials + invented stats = compliance risk.** Regulated colleges (SCPT) restrict advertising claims; a real clinic couldn't ship v1. v2 replaces social proof with *transparency* content (what to expect, fees, FAQ) — which converts better locally anyway.

## 3. v2 decisions

- **Name:** *Wascana Family Physiotherapy* — "Family care, women's health specialists." Wascana is the instant local anchor (the lake every Reginan knows).
- **Palette:** prairie, not spa — warm paper, deep ink, terracotta + sage + wheat gold, one restrained dusty-rose accent (the prairie rose is Saskatchewan's provincial flower; that's the *local* justification for the only pink on the page). No gradients.
- **Type:** Fraunces (editorial serif) + Karla (humanist sans) — chosen for warmth + plain-spoken legibility, not default.
- **Composition:** left-aligned editorial hero with a bottom-line headline; asymmetric service layout with one *featured* service (pelvic health) instead of six equal tiles; native `<details>` FAQ; real trust strip under the hero.
- **Content:** direct-access + insurance + fee-transparency section, "your first visit" consent-forward walkthrough, team bios, communities served, winter/parking note, FAQ, phone-first CTAs, Treaty 4 land acknowledgement in the footer.
- **Accessibility:** skip link, visible focus, 44px touch targets, AA contrast, semantic landmarks, `prefers-reduced-motion`.
- **Honesty:** all names, numbers, addresses, and prices are clearly marked placeholders (README + HTML comments).
