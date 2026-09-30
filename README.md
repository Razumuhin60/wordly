Wordly

Wordly is a free, multilingual, Wordle-style browser game. Guess a five-letter
word in six tries, switch between 12 languages, and start a new round whenever
you want.

## Play Wordly

**[Play Wordly online](https://razumuhin60.github.io/wordly/)**

No download, registration, or installation is required.

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

## How to play

1. Enter a five-letter word using your keyboard or the on-screen keyboard.
2. Submit the word to reveal the result for each letter.
3. Green means the letter is correct and in the right position.
4. Yellow means the letter is in the word but in a different position.
5. Gray means the letter is not in the word.
6. Find the answer within six guesses.

Each round includes one optional letter hint. You can also change the current
word or start a new round immediately after the game ends.

## Run locally

Serve this directory with any static HTTP server. For example, if Python is
installed:

```bash
python -m http.server 4173
```

Then visit `http://localhost:4173/`.

## Deploy with GitHub Pages

1. Upload the project files to the root of a public GitHub repository.
2. Open **Settings → Pages**.
3. Select **Deploy from a branch**.
4. Choose the `main` branch and the `/(root)` folder.
5. Save and wait for GitHub Pages to publish the site.

This repository is published at:

`https://razumuhin60.github.io/wordly/`

## Project structure

```text
index.html                    Game interface, styling, and game logic
words.js                      Generated multilingual word dictionaries
README.md                     Project information and instructions
requirements-wordlist.txt     Word-list generation dependencies
THIRD_PARTY_NOTICES.md        Dataset sources and license notices
```

## Word data

The accepted-guess dictionaries are derived from `wordfreq`. Answer-only
filters use name and place data to prevent proper nouns and location names from
being selected as puzzles. See
[THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md) for source and licensing
details.

## Privacy

Wordly does not require an account and does not send gameplay history to a
server. The selected language and recently played words are stored locally in
the player's browser to remember preferences and reduce repetition.

## Support

If you enjoy Wordly, you can support its development through
[Buy Me a Coffee](https://buymeacoffee.com/razumuhin).
