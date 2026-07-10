# 📚 Reading Vocabulary Notebook

A single-file, offline-friendly **vocabulary & grammar notebook** for study groups —
built with plain HTML/CSS/JavaScript. No server, no framework, no paid services.

**App:** https://mohammadvazirpanah.github.io/vocab-notebook/

> ⚠️ **This public repository contains only the app code.** No vocabulary data is stored here.

## How it works

```
┌─────────────────────┐         ⬇ Update / ⇅ Push          ┌──────────────────────┐
│  Your browser        │ ◄──── GitHub Contents API ────►    │  PRIVATE data repo    │
│  (localStorage)      │        (personal token)            │  words.json           │
│  words + progress    │                                    │  grammar.json         │
└─────────────────────┘                                    └──────────────────────┘
```

- The app runs entirely in the browser; everything you type is stored locally first, so it works offline.
- **⬇ Update** pulls the team's latest words/grammar and merges them in.
- **⇅ Push** does an update first, then shares your additions, edits and review scores.
- Personal spaced-repetition schedules never leave the browser — only score totals are shared.
- Every push is a git commit in the data repo, so the full history is always recoverable.

## Managing it privately with a team

1. Create a **private** repo (e.g. `vocab-notebook-data`) containing `data/words.json` and
   `data/grammar.json` — the app creates them on first push if they don't exist.
2. Invite each team member as a **collaborator** with the **Write** role. This is the entire
   access control: no invitation → no access; remove a collaborator → access ends instantly.
3. Each member creates a **fine-grained personal access token** scoped to *only* that repo
   with **Contents: Read and write**, and enters it once in the app's ⚙ Settings
   (the token is stored only in their browser, is never displayed again, and can only be
   replaced — not removed — from the UI).
4. Point the app at the data repo in ⚙ Settings (`owner/repo`).

## Features

- Quick add with **auto-fill** (free dictionary APIs: definition, IPA, part of speech, examples,
  synonyms, collocations, difficulty, tags) and **bulk add** for whole word lists
- Grammar notes (rule, structure, examples, common mistakes)
- Flashcard review with spaced repetition and session **scores**
- Group tab: per-member contributions, mastery progress and review scores
- Search, filters, unit/topic tags, duplicate detection
- JSON/CSV export, JSON import, light/dark theme, mobile-friendly (Add to Home screen)

## License / reuse

Feel free to fork and adapt for your own study group: replace the default repo name in
`index.html` (`DEFAULT_REPO`) and host via GitHub Pages.
