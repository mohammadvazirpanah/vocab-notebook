# 📚 Reading Vocabulary Notebook

Our shared vocabulary & grammar notebook for reading **Ready for C1 Advanced** (and any other book).
One page, no server, works on laptop and phone.

**👉 Open the app: https://mohammadvazirpanah.github.io/vocab-notebook/**

This public repo contains only the app code. **The group's words and grammar notes live in a
private repo (`vocab-notebook-data`)** — only invited members can read or write them.

## How to join (one-time setup, ~3 minutes)

1. **Open the link above** in Chrome/Firefox — on your phone too.
   - On Android: Chrome menu → **Add to Home screen** → it becomes an app icon.
2. **Accept the collaborator invitation** for the private `vocab-notebook-data` repo
   (check your GitHub notifications/email). This is what authorizes you — no invitation, no access.
3. **Create your GitHub token** (this is your "key" for reading and saving the group data):
   - Go to [github.com/settings/personal-access-tokens/new](https://github.com/settings/personal-access-tokens/new)
   - Token name: `vocab` · Expiration: 1 year
   - Repository access: **Only select repositories** → choose `vocab-notebook-data`
   - Permissions → **Contents → Read and write**
   - Click **Generate token** and copy it (starts with `github_pat_…`)
4. In the app, press **⚙ Settings**: enter your **name** and paste the **token**. Save.
5. Press **⇅ Sync** — you'll get everyone's words, and yours will be shared.

## Daily use

- **＋ Word** — quick form: word + definition is enough. Press **🔎 Auto-fill** to fetch
  IPA, definition, and synonyms automatically. "More fields" has examples, grammar, collocations…
- **＋ Grammar** — save grammar rules from the book: structure, examples, common mistakes.
- **Review tab** — flashcards with spaced repetition. Your review progress is **private**;
  syncing never changes anyone else's study schedule.
- **⇅ Sync** — press it when you start and when you finish adding words. That's it.

## Where is the data?

- The shared lists live in the **private** `vocab-notebook-data` repo as `data/words.json`
  and `data/grammar.json`. Every sync is a commit, so nothing is ever lost.
- Your personal review progress stays in your own browser.
- Deleted your app / got a new phone? Open the link, paste your token, press Sync — everything comes back.
- Extra safety: the ⭳ button in the app exports a full JSON/CSV backup file.

## Rules of the group 🤝

- All definitions and explanations in **clear English only**.
- Anyone can add and edit words and grammar notes.
- Sync before and after a study session to avoid surprises.
