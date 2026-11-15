---
name: brand-report
description: Write a sourced research report on one selected luxury/high-end brand for Sapien Watch, saved to output/<domain>/<brand>/report.md and report.docx. Use after the user picks a brand from the domain-research shortlist, or when asked to write or update a brand report.
---

# Brand report

Read `CLAUDE.md` first. Its rules on sources, prices, counterfeits, and tone apply here.

## Output location
`output/<domain-slug>/<brand-slug>/report.md` (plus `report.docx` once the user approves the content).

## Required sections, in this order

1. **Summary** — 5–7 sentences: what the brand is, why it matters, why viewers should care.
2. **Origin** — founding year, founder or home country, city of origin, heritage story (with sources).
3. **Why it is high-end / expensive** — craftsmanship, production method, materials, brand positioning, pricing strategy. Separate facts from marketing claims.
4. **Materials used in production** — key materials and components, where they come from, and whether the brand publishes this.
5. **Product varieties and portfolio** — main product lines, flagship items.
6. **Price ranges (USD/EUR and approximate LKR)**
   - Table: product line | entry price | flagship price | currency | approx. LKR
   - State the exchange rate used and its date.
   - Mark every LKR figure as approximate.
7. **Where to buy**
   - Countries and regions with official stores or distributors.
   - Availability in Sri Lanka: official store, authorised distributor, online only, or not sold.
8. **Competitors** — 3–5 direct competitors, with one line on how each compares (price, positioning, materials).
9. **Counterfeits: how to tell real from fake** — general, public checks only:
   - Buy only from official stores or authorised sellers. This is the most important rule.
   - Check the brand's official authentication features, such as serial numbers, cards, or packaging, using the brand's own published guide.
   - Be wary of prices far below the normal range.
   - Do not write a guide that helps someone make a convincing fake.
10. **Other things consumers should know** — warranty, care, resale value, sizing or compatibility notes, environmental or labour claims (flag as claims, not facts, unless verified).
11. **Verification status** — list each claim marked Verified / Partly verified / Unverified.
12. **Sources** — numbered list of URLs with the date each was accessed.

## Process
1. Run web searches in parallel for: official brand site, origin and history, pricing, Sri Lanka stockists, counterfeit guidance from the brand, independent reviews.
2. Check at least two independent sources for each important fact (origin, materials, prices).
3. Get the exchange rate from a live source, and write the date next to it.
4. Write `report.md`.
5. Convert to `report.docx` only after the user says the content is approved. Use the `docx` skill for this.
6. End your message with: "Review this report. Reply **approved** to continue to the Sinhala script, or tell me what to change."

## Do not
- Do not state prices without a source and date.
- Do not use hype words ("best ever", "guaranteed", "must-buy").
- Do not add sponsorship or affiliate language.
