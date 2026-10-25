# rawdev-scripter · Studio

A single-file, self-contained web app that turns a rough brief into a ready-to-record Hinglish reel voiceover — in the voice of a faceless Indian creator teaching AI tools, mobile editing and Instagram growth.

No build step, no backend, no API keys. One HTML file, open it and it works.

## What it does

You fill a short brief (tool name, the literal taps, a comment keyword) and it writes the script in three blocks:

1. **Hook** — payoff or pain in the first 3 seconds.
2. **Flow** — the solution as literal taps: *"Sabse pehle… fir… ab niche… bas hogya."*
3. **CTA** — the Triple-Stack, one breath, then the sign-off.

It also prints a live word count with a read-time estimate (target band: 85–130 words / ~35–45s), and three alternative hooks, each a different formula.

## The rules it obeys

Everything in the app comes from the bundled skill (`skill/rawdev-scripter/`):

- **HPSC structure** — hook, problem, solution, CTA, in short comma-joined clauses.
- **Hook library** — 10 formulas (Progression, Secret leak, Capability promise, Negative command, Pain-point diagnosis, Contrarian obituary, Confession / plot twist, Contrarian case study, Vault tease, Shock statistic). The generator picks whichever you select.
- **Voice rules** — Hinglish in Roman script, English tech nouns kept as-is, always *tum / tumhe / tumhara*, house spellings (`krna krlo krdo krlena rkhlo skte ho bas hogya baki toh fir yeh yahan niche`), steps as taps and UI labels, never a greeting opener.
- **Triple-Stack CTA** — comment-keyword → DM, save with a reason, share to a specific person, then *"baki follow bhi krlena"*, then the stretched `byeeeeeeee.......`.
- **Proof & honesty rules** — it never invents statistics, numbers, versions or sources. The shock-statistic hook fires only when the brief supplies both the number and its source; with no proof, the flow falls back to *"result screen pe aa jayega"*.

## Run it

Open `index.html` in any browser. That's it — it's fully self-contained (the only external request is a Google Fonts link, with a system-font fallback so it still looks right offline).

## Publish it on GitHub Pages

1. Create a new repository and push this folder.
2. Settings → Pages → Source: **Deploy from a branch** → Branch: `main` / `/ (root)`.
3. Your studio is live at `https://<your-username>.github.io/<repo>/`.

The `.nojekyll` file is already included so nothing gets filtered out.

## Files

```
index.html                                     the app (this is the artifact)
skill/rawdev-scripter/SKILL.md                 the skill definition
skill/rawdev-scripter/references/voice-and-examples.md   hook library, CTA keywords, voice corpus, gold-standard examples
LICENSE                                        MIT
```

## Notes

- Built as a standalone tool around the `rawdev-scripter` skill. It is a fan/creator tool and is not affiliated with or endorsed by Instagram, Meta, or any of the apps named in the scripts.
- Tool names that appear in examples (Flow AI, Veo 3.1, Omni Flash, CapCut, ChatGPT) are the property of their respective owners and are used descriptively.

## License

MIT — see `LICENSE`.
