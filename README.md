# Wordly

Wordly is a free, multilingual, Wordle-style browser game. Guess a five-letter
word in six tries, switch between 12 languages, and start a new round whenever
you want.

## Play

After enabling GitHub Pages, the game will be available at:

`https://YOUR_USERNAME.github.io/wordly/`

Replace `YOUR_USERNAME` with your GitHub username.

## Features

- Classic five-letter, six-guess gameplay
- 12 languages: English, Turkish, Spanish, German, French, Portuguese, Italian,
  Russian, Arabic, Indonesian, Dutch, and Polish
- 100,000 accepted guesses across all languages
- A curated pool of 500 common answers per language
- Proper names, cities, countries, capitals, and obvious corpus noise excluded
  from random answers
- Physical keyboard and mobile on-screen keyboard support
- Flip, shake, pop, bounce, and confetti animations
- One letter hint per round
- Change-word and instant replay controls
- Recently played words stored locally to reduce repetition
- Responsive dark interface with right-to-left Arabic support
- No backend, account, build step, or paid hosting required

## Run locally

Serve this directory with any static HTTP server, then open `index.html` through
that server. For example, if Python is installed:

```bash
python -m http.server 4173
```

Then visit `http://localhost:4173/`.

## Deploy with GitHub Pages

1. Create a public GitHub repository named `wordly`.
2. Upload the contents of this project to the repository root.
3. Open **Settings → Pages**.
4. Select **Deploy from a branch**.
5. Choose the `main` branch and the `/(root)` folder.
6. Save and wait for GitHub Pages to publish the site.

The live URL will be `https://YOUR_USERNAME.github.io/wordly/`.

## Project structure

```text
index.html                    Game interface, styling, and game logic
words.js                      Generated multilingual word dictionaries
scripts/generate_words.py     Dictionary generation script
scripts/build_answer_exclusions.py
scripts/answer_exclusions.json
requirements-wordlist.txt     Word-list generation dependencies
THIRD_PARTY_NOTICES.md        Dataset sources and license notices
```

## Word data

The accepted-guess dictionaries are derived from `wordfreq`. Answer-only
filters use name and place data to prevent proper nouns and location names from
being selected as puzzles. See [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md)
for sources and licensing details.

## Support

If you enjoy Wordly, you can support its development through
[Buy Me a Coffee](https://buymeacoffee.com/razumuhin).
