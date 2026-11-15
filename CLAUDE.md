# Sapien Watch — content research agent

## Who this is for
The creator behind the YouTube channel and Facebook page **"Sapien Watch"**. Content is short-form and long-form video (Reels, TikTok, Instagram, YouTube, Facebook) that introduces international, high-end brands to **Sri Lankan** viewers, in **Sinhala**.

Goal: build awareness, and grow subscribers and followers. Target output rate: at least 3 pieces of content per week.

## The pipeline (always in this order)
1. **Choose domain** — `domain-research` skill asks which domain to research.
2. **Research top 10 brands** — `domain-research` skill returns 10 trending global brands in that domain and asks the user to pick one.
3. **Brand report** — `brand-report` skill writes the report to `output/<domain>/<brand>/report.md` (and `report.docx`).
4. **Approval gate** — the user reviews the report. Do NOT start the script until the user says it is approved.
5. **Sinhala script** — `sinhala-script` skill writes the voiceover script to `output/<domain>/<brand>/script-*.md`. The user records the voiceover personally.

## Domains
- Apparel, footwear & fashion
- Food & beverage / fast food
- Beauty & personal care
- Travel, airlines & hospitality
- Home, furniture & appliances
- Sports brands

## Rules for all research and content
- **Facts need sources.** Every claim about origin, materials, pricing, awards, or availability needs a source URL in the report's Sources section. If a fact cannot be sourced, write "unverified" next to it.
- **Prices:** show prices in USD or EUR as published, then approximate LKR using a live exchange rate. State the rate and date. Always label LKR as approximate.
- **Availability:** say where the brand is sold in Sri Lanka (official stores, authorised distributors, or online), and say so if it is not sold there.
- **Counterfeits:** describe real-world, public, general checks (stitching, serial or authenticity cards, packaging details, price red flags, buying only from authorised sellers). Never publish a step-by-step guide that helps someone make a convincing fake.
- **No sponsorship language.** The creator is not sponsored by any brand. Do not write sponsored or ad-style claims.
- **Language:** reports in English. Scripts in Sinhala, with brand names in English where that is how Sri Lankans say them.
- **Tone:** factual and calm. No hype like "best ever" or "guaranteed". Write for a general audience, not experts.
- **Users say "approved"** to accept a report. Until then the report is a draft.

## Folder layout
```
output/
  <domain-slug>/
    <brand-slug>/
      report.md
      report.docx
      script-reel-60s.md
      script-youtube-long.md
```
