# Setup guide — Sapien Watch research agent

This guide sets up the workflow on your computer using **Claude Code** (included with **Claude Pro**) and the free tools listed below.

## 1. What you need
| Tool | Purpose | Cost |
|---|---|---|
| Claude Pro | Runs Claude Code and the skills | You already have it |
| Claude Code (CLI) | Runs the agent in this project folder | Included with Pro |
| Git + GitHub | Stores your skills and reports | Free |
| Google Chrome | Lets you check sources and brand sites | Free |
| Google Trends | Checks brand popularity (optional) | Free |
| Exchange rate source (for example xe.com) | Converts USD/EUR to LKR | Free |
| Video editor (CapCut or DaVinci Resolve) | Edits your recorded voiceover | Free versions available |
| Canva (optional) | Thumbnails and text cards | Free tier available |

## 2. Install Claude Code
1. Install Node.js 18 or later from https://nodejs.org.
2. Open a terminal and run:

```bash
npm install -g @anthropic-ai/claude-code
```

3. Check it works:

```bash
claude --version
```

## 3. Log in with your Claude Pro account
From the project folder, run:

```bash
claude
```

Choose the option to sign in with your Claude account (Pro). Use the same email as your claude.ai account.

## 4. Get the project
Clone the repository and switch to the working branch:

```bash
git clone https://github.com/supun-silva/Youtube-agent.git
cd Youtube-agent
git checkout claude/blissful-cray-02l2de
```

## 5. Start a research session
From inside `Youtube-agent`, run:

```bash
claude
```

Then type in plain language, for example:

> Start a new research run for Sapien Watch.

Claude reads `CLAUDE.md`, then the `domain-research` skill asks you to pick a domain. The flow after that is:

1. Pick a domain → you get 10 brands.
2. Pick one brand → you get `output/<domain>/<brand>/report.md`.
3. Read the report. Reply **approved** or ask for changes.
4. After approval → you get `script-reel-60s.md` and `script-youtube-long.md`.

## 6. Keep Claude Pro usage under control
Pro has a usage limit that resets over time. To use it efficiently:
- Run one brand at a time.
- Do the research for the next domain while your recording and editing are in progress.
- Use `/clear` in Claude Code between brands, so old context does not fill up the session.
- Batch the 3 weekly videos: pick 3 brands in one session, then record in one session.

## 7. Your weekly routine (3+ videos)
| Day | Task |
|---|---|
| Monday | Run `domain-research`, pick 3 brands, generate and approve 3 reports |
| Tuesday | Generate the Sinhala scripts for all 3 |
| Wednesday | Have a native Sinhala speaker review the scripts (or review them yourself) |
| Thursday | Record voiceovers |
| Friday | Edit and publish: 1 Reel, 1 TikTok, 1 YouTube, 1 Facebook post |

## 8. Editing and publishing
- Import your voiceover into CapCut or DaVinci Resolve.
- Add product images or video that you have the right to use. Use official brand press images where the brand allows it, or your own footage.
- Export a 9:16 version for Reels, TikTok, and Shorts, and a 16:9 version for YouTube and Facebook.
- Post the same clip to Instagram, TikTok, YouTube Shorts, and Facebook Reels. Post the long version to YouTube.

## 9. Things to keep in mind
- **Sources:** Check the source links in each report before recording.
- **Images:** Do not use brand images unless you have the right to use them.
- **Prices:** LKR prices change. Check them again the day you publish, and say "approximate" on screen.
- **Sinhala quality:** Have a native speaker review each script before recording.
- **Git:** Commit the `output/` folder after each approved report so you have a history:

```bash
git add output
git commit -m "Add approved report: <brand>"
git push -u origin claude/blissful-cray-02l2de
```

## 10. Optional tools to add later
- **Google Drive:** back up `output/` and your recordings.
- **Google Sheets:** a content calendar with columns for brand, domain, status, and publish date.
- **Metricool** or **Meta Business Suite:** schedule posts to Facebook and Instagram (free tiers available).
- **Later.com** or **TikTok native scheduler:** schedule TikTok posts.
