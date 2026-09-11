# Periodic Table Practice

A single-page web app for drilling atomic numbers against the full 118-element periodic table, with element names shown in Traditional Chinese (繁體中文).

**[Try it live](#)** — once GitHub Pages is enabled (see below), replace this link.

## How it works

Pick a practice scope, then answer with the atomic number for each element shown:

- **依族練習** — drill one group/column at a time (CAS-style groups 1A–8A and 1B–8B, with 8B covering IUPAC groups 8–10, plus 鑭系/Lanthanides and 錒系/Actinides)
- **依週期練習** — drill one period/row at a time (Periods 1–7)
- **自訂範圍** — set a custom atomic-number range (e.g. 5–30)
- **Zen 模式 ∞** — all 118 elements, unfiltered

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
