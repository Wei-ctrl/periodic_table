# Periodic Table Practice

A single-page web app for drilling atomic numbers against the full 118-element periodic table, with element names shown in Traditional Chinese (繁體中文).

**[Try it live](#)** — once GitHub Pages is enabled (see below), replace this link.

## How it works

The start screen is a Taiwan-style periodic table (CAS group labels 1A–8A / 1B–8B with 8B spanning IUPAC groups 8–10, periods 1–7, and separate 鑭系/錒系 rows, tinted by 金屬 / 類金屬 / 非金屬). Build your practice set by tapping:

- individual elements
- a group header (e.g. **1A**) to toggle the whole column
- a period number (**1**–**7**) or the **鑭系** / **錒系** label to toggle the whole row
- **全選** / **清除** for everything or nothing

Your selection is remembered between visits. Press **開始練習** and answer with the atomic number for each element shown. A **中 / EN** toggle switches the prompt between the Chinese name and the element symbol, and the speaker button reads the name aloud (Mandarin or English) using the browser's speech synthesis.

Answers are entered on an on-screen numpad. A correct answer briefly reveals the atomic number and auto-advances to the next question; an incorrect one shows the right answer and waits for you to retry or skip ahead.

## Tech

Vanilla HTML/CSS/JS, no build step, no dependencies. Everything lives in `index.html`.

## Running it

Just open `index.html` in any browser — locally, or after cloning:

```
git clone <this-repo-url>
cd periodic-table-practice
open index.html   # or double-click it
```

## Hosting on GitHub Pages

Settings → Pages → Deploy from branch → `main` → `/ (root)`. The app will be live at `https://<your-username>.github.io/<repo-name>/`.
