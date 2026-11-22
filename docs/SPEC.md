# BuyOrBye: Spec

**Buy less, buy better** · #15 of 32 · Wave 2: Recurring keepers · Used: Weekly · Very easy · Revenue potential: Medium · Money & Work · Source: ChatGPT (reworked; was WorthIt)

## One-liner

A purchase-decision companion, not just a calculator. Before you buy: compare unit prices, work out cost-per-use, check monthly vs annual. Tempted? Put it on a cool-off wishlist and BuyOrBye checks back in 7 or 30 days. Already bought it? Log each use and watch the cost-per-use fall, so you can see what was really worth it.

## Problem / audience

- **Who it's for:** Shoppers comparing pack sizes, people trying to stop impulse buying, anyone deciding whether a big purchase or subscription is worth it.
- **The problem it solves:** Impulse buys and confusing prices. People rarely know whether something was worth it, and unit prices and multi-buy deals are hard to compare in the aisle.
- **Example:** A user wants £120 trainers, adds them to a 30-day cool-off, says 'no' when asked a month later, and £120 goes into their saved total. They also log gym visits and watch the membership drop from £40 to £4.44 a visit.

## MVP features (ship with only these)

1. Calculators: price-per-unit with mixed units, cost-per-use, monthly vs annual break-even, discounts and multi-buys
2. Cool-off wishlist: add an item, pick 7 or 30 days, get asked 'still want it?'
3. 'Saved by not buying' running total for the things you skipped
4. Cost-per-use tracker: log uses of things you bought (gym, coat, coffee machine) and watch the cost per use drop
5. Shareable cards: 'The 1 kg bag is 23% cheaper', 'I saved £340 by waiting'

## Not in MVP

- Purchase history and a yearly 'was it worth it' recap
- Deal and alternative links (affiliate), clearly labelled
- Home-screen widget for the cool-off list

## Monetisation

| Model | Detail |
|---|---|
| Free | All calculators and a small wishlist, with ads |
| Premium | £1.99/month or £9.99 lifetime: unlimited wishlist and tracked items, history, recap, no ads |
| Ads | AdSense on the web calculators, AdMob in the app |
| Affiliate | Deal and alternative links, clearly labelled |

Prices are starting points; test before committing. **Portfolio premium promise:** free has ads; the moment you pay you get no ads, cloud backup and storage, and sync across your devices, plus this app's extras.

## Retention: The Progression Loop

| Stage | Design |
|---|---|
| Cue | Cool-off check-ins the user scheduled; 'log a use' prompts |
| Tiny win | Answer 'still want it?' or log a use in one tap |
| Progress | Saved-by-not-buying total; cost-per-use falling |
| Share | Savings and comparison cards |
| Next step | Monthly recap of what was worth it |
| Cadence | Weekly + whenever shopping |

Follow the portfolio guardrails: no guilt-trip notifications, no fake urgency, progress is
never wiped, at most one notification a day by default.

## Animation and tone: five signature animations

**Playful.** Celebrations, confetti, cute characters, satisfying sounds and mild comic reactions. Nothing tragic.

- Item skipped: it waves 'bye!' and walks off screen as the savings jar fills
- Cool-off check: the item gives you puppy-dog eyes ('still want me?')
- Cost-per-use drops: the price tag deflates like a balloon
- Unit-price win: two packs face off in a boxing ring and the cheaper one wins
- Impulse resisted milestone: the stickman flexes in front of the shop window


## AI

**None.** Not needed. Plain code does everything this app does. (Portfolio rule: plain code first, code does the maths,
cheapest model, shared budget cap, premium-gated.)

## Platform & data

- **Platform:** Calculators ship first as free web pages (SEO); the app adds the wishlist and tracking.
- **Data:** On the device only.
- **Backend:** None for the free version: everything lives on the phone. Premium backup and sync use the shared portfolio backend (see the master repo's HOSTING.md).
- **Stack:** shared portfolio foundation (Expo, PostHog, RevenueCat, AdMob, shared Progression Loop module).

## Growth engine

- **Content pillars:** Unit-price traps; Cost-per-use thinking; Impulse buying and cooling off; Subscription maths; Deal myths
- **Shareable output:** Savings and comparison cards

## Risks

A calculator on its own is a weak business; the wishlist and tracking are what make this an app. Affiliate links must never bias the 'is it worth it' answer.

## Launch checklist

- [ ] Name checked on the App Store, Play Store and a trademark search
- [ ] MVP features done and tested
- [ ] Progression Loop wired (cue, tiny win, progress, milestone, next step)
- [ ] Privacy policy and terms
- [ ] Landing page
- [ ] Analytics wired (D1/D7/D30 retention)
- [ ] Payments / ads wired
- [ ] Added to the Growth & Maintenance Engine as an app config
