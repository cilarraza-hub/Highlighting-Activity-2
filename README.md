# Text Highlighter and Categorizer

An interactive reading activity where learners highlight passages of text and assign each one to a category. The tool checks the selection against an answer key and gives immediate "Correct!" / "Try again!" feedback.

The activity uses an excerpt about the gender citation gap in academic research, split into three passages, each mapping to one category.

## How it works

1. **Select text** — click and drag across any portion of the passage. The selection is highlighted in yellow.
2. **Pick a category** — click the highlight to open a menu, then choose **Background**, **Compare**, or **Connect**.
3. **Get feedback** — the highlight recolors to match the category, and the result area shows whether the selection was correct.
4. **Remove a highlight** — double-click it.

A selection is marked **correct** when it falls anywhere within the target passage for the chosen category. Introductory lead-in sentences that sit outside the target range are treated as incorrect.

## Categories and colors

| Category   | Color | Passage |
|------------|-------|---------|
| Background | Peach (`#FFF4CC`) | Paragraph 1 |
| Connect    | Green (`#D9FDD3`) | Paragraph 2 |
| Compare    | Blue  (`#CCE5FF`) | Paragraph 3 |

The legend at the top of the page shows the color for each category.

## Running it

This is a single self-contained HTML file with no dependencies or build step.

- **Locally:** open `index.html` in any modern web browser.
- **GitHub Pages:** push this repository, then enable Pages under *Settings → Pages* and select the branch. The site will be served from `index.html` automatically.

## Files

- `index.html` — the complete activity (HTML, CSS, and JavaScript in one file).
- `README.md` — this file.

## Notes and known limitations

- The passage area is editable (`contenteditable`), so text can be changed as well as highlighted. Because the answer check compares the selected text to the on-screen passage, edits can affect matching.
- The answer key is embedded in the page source and is visible to anyone who views the source.
- Matching ignores case, punctuation, and spacing, and compares the remaining letters and numbers.

## Possible future improvements

- Keyboard access for selecting text and choosing a category, so the activity works without a mouse.
- Legend cues beyond color (labels, patterns, or icons) for users who can't distinguish the colors.
- A read-only mode so the passage can be highlighted but not edited.
