# Periodic Table Practice

A single-page web app with three Traditional Chinese (繁體中文) chemistry drills: atomic numbers across the full 118-element periodic table, classifying substances as elements, compounds, solutions, or other mixtures, and writing the chemical formula for a named compound.

**[Try it live](#)** — once GitHub Pages is enabled (see below), replace this link.

## How it works

A tab bar at the top switches between the three practice modes.

### 原子序練習 (atomic number practice)

The start screen is a Taiwan-style periodic table (CAS group labels 1A–8A / 1B–8B with 8B spanning IUPAC groups 8–10, periods 1–7, and separate 鑭系/錒系 rows, tinted by 金屬 / 類金屬 / 非金屬). Build your practice set by tapping:

- individual elements
- a group header (e.g. **1A**) to toggle the whole column
- a period number (**1**–**7**) or the **鑭系** / **錒系** label to toggle the whole row
- **全選** / **清除** for everything or nothing

Your selection is remembered between visits. Press **開始練習** and answer with the atomic number for each element shown. A **中 / EN** toggle switches the prompt between the Chinese name and the element symbol, and the speaker button reads the name aloud (Mandarin or English) using the browser's speech synthesis.

Answers are entered on an on-screen numpad. A correct answer briefly reveals the atomic number and auto-advances to the next question; an incorrect one shows the right answer and waits for you to retry or skip ahead.

### 物質分類練習 (substance classification practice)

A 185-item bank covering the standard 國中 curriculum, shown with both their Chinese name and English translation, drilled against four categories:

- **元素** (element, 49 items) — gases (氫氣, 氦, 氯氣…), liquids (溴, 汞), solid nonmetals (碘, 矽, 鑽石…), and metals (鈉, 鐵, 24K金…)
- **化合物** (compound, 89 items) — oxides, acids, bases, salts, and organic compounds (水, 二氧化碳, 硫酸, 氫氧化鈉, 食鹽, 葡萄糖…)
- **溶液** (solution, a homogeneous mixture, 33 items) — aqueous solutions, gas mixtures, and alloys (鹽水, 空氣, 黃銅, 不鏽鋼…)
- **其他混合物** (other, heterogeneous mixture, 14 items) — 牛奶, 泥沙水, 花崗岩, 土壤…

The set deliberately includes the classic 純物質 vs 混合物 "trap pairs" that sound alike but aren't — 過氧化氫 (compound) vs 雙氧水 (solution), 氯化氫 (compound) vs 鹽酸 (solution), 24K金 (element) vs 14K金 (solution alloy), 蒸餾水 (compound) vs 自來水 (solution), and more.

Toggle which categories to include with the colored chips (at least one must stay selected), then tap the matching category button for each item — or press **1**–**4** on a keyboard. A correct answer auto-advances; a wrong one highlights the right category and waits for **下一題**.

### 化學式練習 (chemical formula practice)

An 84-item bank of compounds grouped into six chip-filterable categories — 氧化物 (oxides), 氫化物 (hydrides/water), 酸 (acids), 鹼 (bases), 鹽類 (salts), 有機物 (organics). Shown a Chinese name (e.g. 二氧化氮), type the chemical formula (e.g. `NO2`) into the text field — matching is case-insensitive and ignores whitespace, so `no2` also works. Quick-insert buttons handle `(` and `)` for formulas like `Ca(OH)2` or `Fe(NO3)2` without switching keyboards, plus a backspace and a 清除 (clear) button that also resets a wrong answer for another attempt. Press Enter to submit or advance.

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
