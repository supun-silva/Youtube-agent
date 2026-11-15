---
name: sinhala-script
description: Write a Sinhala voiceover script for an approved Sapien Watch brand report, as a 60-second Reel script and a long-form YouTube script, for the creator to record personally. Use only after the user has replied "approved" to a brand report.
---

# Sinhala voiceover script

## Precondition
Only run this after the user has approved the brand report (replied "approved"). If the report is not approved, stop and say so.

Read `CLAUDE.md` and the approved `output/<domain>/<brand>/report.md`.

## Who records it
The creator records the voiceover personally. Write the script so it is easy to read aloud: short sentences, natural spoken Sinhala, and no tables or bullet points in the spoken text.

## Outputs

### 1. `script-reel-60s.md` — about 60 seconds spoken
- Hook (first 3 seconds): one striking fact from the report, in Sinhala.
- Body: 3 short points — what it is, why it's expensive, one thing to know before buying.
- Close: a call to follow the channel for the full video.
- Length target: about 120–150 Sinhala words.

### 2. `script-youtube-long.md` — about 8–10 minutes spoken
- Intro (30 seconds): who, why this brand.
- Sections matching the report: origin, why it's high-end, materials, product range, prices in LKR, where to buy in Sri Lanka, competitors, how to spot fakes, other things to know.
- Outro: summary and call to subscribe.
- Length target: about 1,100–1,400 Sinhala words.

## Format for each script
Use a simple table or numbered blocks so the creator can follow it while recording:

```
[00:00–00:03] HOOK
Spoken Sinhala text here.
(On screen: ...)

[00:03–00:15] POINT 1
...
```

Include on-screen text cues in brackets, such as product images or price cards.

## Language rules
- Write in Sinhala. Keep brand names and technical terms in English where Sri Lankans normally use them (for example "Rolex", "Louis Vuitton", "GPS").
- Give Sinhala spellings or phonetic hints for hard brand names in a short pronunciation list at the top of each script.
- Write prices as "රුපියල් ..." with the approximate LKR figure and "ආසන්න" (approximately).
- Keep the tone factual and calm, with no hype.

## Checks before finishing
- Every fact in the script matches the approved report.
- No sponsorship language.
- The script states prices as approximate.
- Say at the top of your message that the creator should have a native Sinhala speaker review the script before recording, because AI-written Sinhala can sound unnatural or misuse technical terms.
