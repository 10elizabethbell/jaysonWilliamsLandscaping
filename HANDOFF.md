# Jayson Williams Landscaping — handoff at ~60%

**Live:** https://10elizabethbell.github.io/jaysonWilliamsLandscaping/ · **Repo:** https://github.com/10elizabethbell/jaysonWilliamsLandscaping · **Built:** 2026-10-19 from Muse brief (run 2026-10-19, FB group "NJ Seeking Contractors" ad post)

## What's built
- **One page,** `index.html`, 47 KB, with no photos and no web fonts. The page is drawn by code, so it loads fast on cellular. Only the og image and the iPhone icon are in `assets/`.
- **Sections, in order:**
  - header: wordmark, and tap-to-call 609-937-8650 top right
  - hero: "Your yard. Our work.", their pride line, orange "Get a free quote" and outlined "Text us"
  - What we do: 6 service rows
  - Getting a quote: 3 steps
  - a grass divider
  - "Get a free quote." form, under "Now booking new customers in New Jersey & Pennsylvania."
  - closing slogan "Your yard. Our work. Your satisfaction." over a second lawn
  - footer: name, services, phone, email
- **The world: a fall lawn.**
  - Spruce green (#12302a) for the dark sections, dew-light (#edf2e6) for the services section.
  - Mower orange (#ef7d2d) is the one action color, and it's also the mower.
  - A mulch bed with a wavy, hand-cut edge borders the lawn.
- **The signature is a lawn you mow yourself.**
  - It starts as shaggy tall grass with fall leaves on it.
  - An orange push mower drives itself in rows, cutting real light/dark mowing stripes (the stripe follows the direction it drives), spraying clippings, and mulching leaves into orange bits.
  - Touch or mouse over the lawn and the mower follows your finger or cursor in any direction. A vertical drag on a phone mows; it doesn't scroll the page or trigger pull-to-refresh.
  - It drives itself again 2.5 seconds after you let go.
  - Cut grass grows back, and new leaves keep drifting in.
  - Tall tufts sway in wind gusts and part around the mower.
- **The lawn is carried through the page:**
  - the hero lawn
  - a grass strip between the services and the form that parts under your finger and has a few leaves in it
  - a mowable patch beside the form (desktop only)
  - the closing lawn
  - Ticking a service in the form throws a small puff of clippings (leaf bits for Leaf removal).
- **Contact:**
  - "Text us" opens `sms:+16099378650` with "Hi Jayson Williams Landscaping! I'd like a free quote for my yard."
  - The form has service chips, address or town, name, and notes. It checks that town and name are filled in, then opens a pre-written text listing the work, town, name and notes. Tested: `&`, quotes, `#` and line breaks all come through.
  - Tapping a service row ticks that service in the form and scrolls there.
- **Tunables** are in `CFG` at the top of the lawn script:
  - `HOLD`/`GROW`: how long stripes last
  - `DECK`: mower size
  - `SPEED`, `TURN`, `IDLE`: how the mower drives
  - `WIND`: grass sway
  - `PUSH`, `K`, `D`: how the grass parts and springs back
  - `LEAVES`: leaf count
  - `PREMOW`: how much is mowed before the first frame

## Assumptions I made
- **"We", not "I".** Their ad and captions speak as "we".
- **The owner is unknown.** The ad was posted from a personal profile, "Brooks Will", and the brief can't confirm how that person relates to the business. No name appears on the site.
- **Service names are split into short items** from their four verbatim lines: Lawn care, Landscaping, Yard cleanups, Leaf removal, Hedge trimming, Mulching. "Residential & Commercial" became "For homes and businesses."
- **Hero headline** is their own slogan, cut to "Your yard. Our work."; the full slogan is the close. The promise line is their caption, word for word.
- **Step copy is mine,** built on their words:
  - "We'll tell you plainly what it takes to get your yard right."
  - "Professional service and quality work, done the way we'd want it done on our own yard."
- **Colors are my choice.** They have no logo or brand colors. Orange was picked to stand apart from the earlier landscaper sites (Zelaya's lime, Los Compas's gold).
- **Favicon and iPhone icon are a "JW" monogram over mowing stripes.** There's no logo to take a mark from.
- **Not treated as a 40+ audience.** Nothing in the brief says so, so the full motion is on.
- **The world is the runner-up pick.** Impeccable's roll (seed bfcfc61a) assigned candidate 6. I overrode it with the pitch-site rule to pick the world that best carries a touchable signature.

## Placeholders and gaps
- **No Facebook link anywhere.** The only links are a group post, which needs membership, and the poster's personal profile, which isn't confirmed as the business. I didn't want to send customers to someone's personal page. Add the business page's link under the steps and in the footer once we have it.
- **No photos, logo, reviews, prices, hours or towns.** The page says nothing about them. Without photos, the work section is replaced by the steps.
- **Service area is only "New Jersey & Pennsylvania".**

## Questions for the owner
1. Is there a Facebook business page (or Instagram) to link? Who should the site name: Jayson, Brooks, or neither?
2. Photos of real jobs, especially fall cleanups and before/after lawns? They'd go in as proof, framed in the lawn.
3. Which towns or counties do you cover?
4. Do you answer texts quickly enough for text to be the main way to book? (The ad says "call or text", so I built it that way.)
5. Any services missing: snow removal, gutters, sod, planting?
6. Hours, or "same-week" availability you'd want to promise?
7. A logo or truck lettering we should match?

## Ideas not built (yours to pick)
- **Runner-up world: hedge trimming.** A shaggy hedge your finger clips into a crisp shape with shears, with clippings falling.
- **Service rows vs. form chips (a judgment call).** On a 1440×900 screen, the six service rows and the six form chips can both be in view. They do related things: a row ticks its chip and scrolls to the form. Ellie's rule is "no two controls doing the same thing in view." The alternative is the house text-to-book module: each row opens its own pre-filled text naming the service.
- **A mini mower on the divider strip** that mows it as it scrolls into view.
- **The closing lawn shows the stripes you mowed in the hero.**
- **The hero lawn's bottom edge** could get a ragged grass fringe instead of a straight edge.
- **A short vibration when your finger mulches a leaf** (works on Android only).
- **Fonts:** a display face could replace the system stack if Ellie wants more character. The Impeccable detector flags the system font, but it's the house rule.
- **When photos arrive,** a before/after slider with a plain orange divider, under the services.

## Not verified
- Real-device touch on an iPhone and on Android, and inside Facebook's in-app browser. Tested here with Playwright Chromium (real CDP touch drag) and WebKit at 320, 360, 390, 414, 430 and 1440, plus landscape-phone CSS.
- Whether the SMS hand-off really opens Messages on iOS and Android. The `sms:` URLs and their bodies were captured and decoded in Chromium.
- Frame rate on real older phones. Simulated in Chromium at 390px, 3× pixel density and 4× CPU throttle: frames take 26.6ms median and 34ms at the 90th percentile, about 30–38fps. That was 57ms before the mask-blur fix. Load under the same throttle takes about 1.5s. If it stutters on a real phone, lower the canvas pixel ratio to 1.5 on touch screens, or skip every other stripe-mask rebuild.
