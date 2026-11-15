---
name: domain-research
description: Ask the user which domain to research, then find the top 10 trending global luxury/high-end brands in that domain and let the user pick one. Use when the user wants to start research, pick a domain, or find brands to feature for Sapien Watch.
---

# Domain research

## Step 1 — Ask for the domain
Ask the user to pick one domain from this list (numbered):
1. Apparel, footwear & fashion
2. Food & beverage / fast food
3. Beauty & personal care
4. Travel, airlines & hospitality
5. Home, furniture & appliances
6. Sports brands

Do not continue until the user answers.

## Step 2 — Research top 10 brands
Use web search. Run several searches in parallel, for example:
- "top luxury [domain] brands [current year]"
- "most searched [domain] brands [current year] trend"
- "[domain] brands available in Sri Lanka"
- "Google Trends [domain] brands" (note the results are indicative only)

Rank candidates by:
1. **Global popularity** — recognised worldwide and mentioned in multiple independent rankings.
2. **Current trend** — recent press, sales growth, or social buzz within the last 12 months.
3. **Sri Lankan relevance** — sold in Sri Lanka, or strongly searched or known by Sri Lankan consumers. Brands with no Sri Lankan presence still count, but flag them as "not sold locally".

Pick the top 10. For each, give:
- Brand name and country of origin
- One-line reason it's trending
- Availability in Sri Lanka (Yes / Via online only / Not sold locally)
- 1–2 source links

## Step 3 — Let the user pick
Present the 10 brands as a numbered table and ask: "Which brand should I write the report on?"

When the user picks one, save a short `output/<domain-slug>/shortlist.md` with the 10 brands and sources, then hand off to the `brand-report` skill.

## Notes
- If web search returns thin or old results, say so and tell the user which rankings you could not verify.
- Never invent brands, rankings, or sources.
