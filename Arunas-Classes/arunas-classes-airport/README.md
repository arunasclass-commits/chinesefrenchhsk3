# Aruna's Classes — Airport 机场 (New HSK 3)

An interactive Mandarin Chinese revision app used in **Aruna's Classes** to reinforce
listening, reading, speaking and writing after each lesson.

© 2026 **RRAruna Enterprises** · ChineseFrench · Aruna's Classes — Foreign Languages.
All Rights Reserved. Made in India 🇮🇳

## What it does

A single, self-contained web app (`index.html`) covering one lesson's vocabulary:

- **Vocabulary** — picture + character + pinyin + meaning, audio, and character etymology (字源).
- **Writing** — animated stroke order, then write each character **3 times** with a mistake-based score and sound.
- **Listening** — hear a word in Mandarin and choose the correct characters (no pinyin).
- **Reading** — read Chinese sentences (no pinyin) and answer multiple-choice questions in Mandarin.
- **Speaking** — model audio plus an optional microphone pronunciation check.

Current lesson: **Airport / 机场** (17 words, aligned to New HSK 3 vocabulary).

## Run it

Open `index.html` in a modern browser (Chrome or Edge recommended for voice and
microphone features). An internet connection is required — the stroke-order
animations load character data from a public CDN.

## Live hosting (GitHub Pages)

1. Push this folder to a GitHub repository.
2. **Settings → Pages → Source: `main` branch → Save.**
3. Because the file is named `index.html`, your site is served at
   `https://<username>.github.io/<repo-name>/`.

## Make the next lesson

The app is content-driven. Open `index.html`, find the `LESSON` object near the top
of the `<script>` block (marked *"ARUNA: edit ONLY this"*), and replace the `vocab`
and `reading` entries. Every module rebuilds automatically. Keep the same structure:

```js
{ w:"机场", p:"jīchǎng", m:"airport", pic:"🛫", ety:"字源 explanation..." }
```

## Credits & technology

- Stroke order and writing quiz: [Hanzi Writer](https://hanziwriter.org/) (MIT-licensed library).
- Audio and pronunciation: the browser's built-in Web Speech API.
- Lesson content, teaching method, etymology notes and app design are the intellectual
  property of RRAruna Enterprises.

## License

All Rights Reserved. See [LICENSE](LICENSE).
