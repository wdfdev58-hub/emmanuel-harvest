# Emmanuel Harvest Christian Fellowship — brand & build notes

## Origin
Lovable rebuild (CLAUDE.md §0 case B). Original: https://emmanuelharvest.lovable.app/
Real content captured from operator screenshots on 2026-07-19.

## Brand
- Full name as they style it: **Emmanuel Harvest Christian Fellowship** (short: Emmanuel Harvest)
- Palette: `gold` (ink/ash/coal + ember/blaze/gold + bone) — kept from v1, it already reads as
  golden harvest light at sunset and matches the church's real hero photo style.
- Type: Fraunces (display/scripture, incl. italic accent) + Inter (body/UI) — kept from v1.
- Logo: original site used a simple line-drawn plus/cross mark next to the wordmark. Recreated as
  an inline SVG (`brand-mark`, nav + footer) rather than scraping a low-res screenshot crop — same
  shape, in the site's gold rather than the original's blue, with a soft pulse glow.
- Hero image (`assets/img/hero.jpg`): a single worshipper, arms raised, backlit by the sun — this
  is an exceptionally close match to the original Lovable hero's "raised hands at sunset" feel, so
  it was kept as-is rather than refetched.

## Real content carried over (verbatim from the operator's brief / screenshots)
- Tagline: "A place of worship, growth, and community." (hero subtext)
- Welcome paragraph (Welcome section)
- Vision + Mission (new `#vision` section, two cards, full verbatim text)
- Core Values — Love / Truth / Wisdom / Transformation (new `#values` section, verbatim
  descriptions from the old site's "Our Core Values" block)

## The signature moment: "Beyond Sunday" (`#beyond`)
This church's story is unusual — the vision explicitly names *industries* and *nations*, not just
community, and the mission calls out entrepreneurial excellence alongside discipleship. That's the
one thing this site needed to say loudly. Built a dedicated section: a two-row CSS marquee (opposite
directions, pure CSS `translateX` loop, no JS) cycling through the spheres the vision names —
Business, Government, Education, Technology, Media, Arts, Enterprise / Community, Healthcare,
Innovation, Leadership, Industry, Nations, Family, Marketplace — bracketed by the exact "transform
communities, industries, and nations…" line from their vision statement. Respects
`prefers-reduced-motion` (animation removed, list still readable).

## Contact details / service times — deliberately NOT invented
Both the old Lovable site (123 Faith Avenue, Grace City; (555) 123-4567; Sun 9 & 11, Wed 6:30, Fri 7)
and our own generator's default template (Sunday 09:00, Wednesday 18:00, Friday 18:30,
`tel:+27000000000`) ship the same kind of plausible-looking but fabricated specifics. Neither was
confirmed by the operator's screenshots, so **none of it was carried across**. The Times & Place
section now reads "Service times — coming soon," the fake `tel:` link was removed from the Visit CTA
(replaced with a "Meet Pastor Noble" anchor), and only the confirmed city/province (Mangaung, Free
State) is used for location/map. Fill these in for real the moment the church confirms them.

## Repurposed sections (grounded in real text, not invented)
- **Get involved** grid (`#involved`): renamed from generic "Ministries" (Prayer & Intercession /
  Worship & Praise / Youth on Fire / Community Outreach — none of which were confirmed) to the four
  pillars stated directly in the real mission text: Discipleship, Leadership Development, Kingdom
  Enterprise, Next Generation. No invented program names.
- Welcome section's stat row changed from an invented "3 weekly gatherings" count to
  Disciples / Leaders / Nations, sourced from the mission sentence ("build disciples, develop
  visionary leaders… transform communities, industries, and nations").

## Motif notes
- Kept the gold particle canvas ("ember field" in `js/main.js`) as ambient atmosphere — reads as
  rising light/pollen against a sunset hero, works for both churches named "fire" and "harvest."
  Shifted the visible copy away from fire language: eyebrow icon 🔥 → 🌾, "Fuel the fire" → "Sow into
  the harvest," "there's room at this fire" → "there's room here."
- Section order: Hero → Welcome → Vision & Mission → Scripture (Matthew 9:37, harvest) → Beyond
  Sunday (signature) → Core Values → Moments gallery → Times & Place → Get Involved → Visit CTA → Give.
