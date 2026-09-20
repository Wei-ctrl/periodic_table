# Periodic Table Practice

A single-page web app with two Traditional Chinese (繁體中文) chemistry drills: atomic numbers across the full 118-element periodic table, and classifying substances as elements, compounds, solutions, or other mixtures.

**[Try it live](#)** — once GitHub Pages is enabled (see below), replace this link.

## How it works

A tab bar at the top switches between the two practice modes.

### 原子序練習 (atomic number practice)

The start screen is a Taiwan-style periodic table (CAS group labels 1A–8A / 1B–8B with 8B spanning IUPAC groups 8–10, periods 1–7, and separate 鑭系/錒系 rows, tinted by 金屬 / 類金屬 / 非金屬). Build your practice set by tapping:

- individual elements
- a group header (e.g. **1A**) to toggle the whole column
- a period number (**1**–**7**) or the **鑭系** / **錒系** label to toggle the whole row
- **全選** / **清除** for everything or nothing

Your selection is remembered between visits. Press **開始練習** and answer with the atomic number for each element shown. A **中 / EN** toggle switches the prompt between the Chinese name and the element symbol, and the speaker button reads the name aloud (Mandarin or English) using the browser's speech synthesis.

Answers are entered on an on-screen numpad. A correct answer briefly reveals the atomic number and auto-advances to the next question; an incorrect one shows the right answer and waits for you to retry or skip ahead.

### 物質分類練習 (substance classification practice)

A bank of 48 everyday substances (12 each), shown with both their Chinese name and English translation, drilled against four categories:

- **元素** (element) — e.g. 金, 氧氣, 鑽石
- **化合物** (compound) — e.g. 水, 二氧化碳, 純氯化鈉
- **溶液** (solution, a homogeneous mixture) — e.g. 鹽水, 海水, 空氣, 黃銅
- **其他混合物** (other, heterogeneous mixture) — e.g. 花崗岩, 什錦沙拉, 混凝土

Toggle which categories to include with the colored chips (at least one must stay selected), then tap the matching category button for each item — or press **1**–**4** on a keyboard. A correct answer auto-advances; a wrong one highlights the right category and waits for **下一題**.

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
