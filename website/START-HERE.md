# Vibe-coding this website with Claude

## 1. Open the folder in Claude Code
1. Open the Claude desktop app and go to the **Code** tab.
2. Choose this folder: `C:\35 Budhas\website`
3. Claude reads `CLAUDE.md` first, so it already knows the project. You don't need to explain it again.

## 2. The loop
1. **Ask** for one change in plain words.
2. **Look**: open `index.html` in your browser and refresh.
3. **React**: "the button is too small", "I like it, now…", "undo that".

Small steps work better than one big request. If something breaks, say "that broke X, please fix it" or "undo the last change".

## 3. Prompts to try (copy, then adjust)

**Warm-up (5 min)**
- "Make the title bigger on phones and add a short subtitle under it in both languages."
- "Change the gold accent color to a deeper saffron. Check dark mode still looks good."

**Learning features**
- "Add a 'Glossary' button. When tapped, show short plain explanations of: eon, arhat, Sangha, stupa, Dharma, bodhisattva, vow. Both languages."
- "In the Buddha popup, add a 'Did you know?' line with one fact about the object they hold (sword = cutting ignorance, lotus = purity…). Ask me before writing facts you're not sure about."
- "In Practice mode, add an optional soft bell sound when I tap Bow, with a mute button."

**Game ideas**
- "Add a third question type to the matching game: 'Which direction does this Buddha sit in?' with 4 choices."
- "Add a timed 'speed round' of 10 questions."

**Before sharing**
- "Check the whole page on a 390px phone screen and list anything that looks broken. Then fix it."
- "Read CLAUDE.md 'Still open' and tell me what is left before this site is ready to publish."

## 4. Tips from a facilitator's view
- Say **who** it's for in your prompt: "for a 12-year-old who has never been to a temple".
- Ask Claude to **explain** before it builds: "Suggest 3 ways to do this, don't code yet."
- When it works, ask: "What did you change and why?" That's how you learn the code.
- Keep a copy before big changes (copy the folder, name it `website-backup`).

## 5. Putting it online later
The site is just files, so free hosts work: GitHub Pages, Netlify Drop (drag and drop the folder), or Cloudflare Pages. Ask Claude Code: "Help me publish this folder on GitHub Pages step by step."
