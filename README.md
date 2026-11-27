# uplift-question-bank

Question data for the UPLIFT game. Edit JSON only; the game picks changes up without a rebuild.

- `manifest.json` — `version` + map of category → URL. Replace `Khanzyoxxreal` with your GitHub username, and **bump `version` after every change**.
- `questions/*.json` — arrays of `{ "question", "answer" (number > 0), "unit", "category" }`.
- Each category needs ≥ 7 valid unique questions.

URL format: `https://cdn.jsdelivr.net/gh/Khanzyoxxreal/uplift-question-bank@main/manifest.json`

## Optional `label` field (V1.1)
Add `"label": "Jupiter diameter"` to a question to let the game use it in **Sort it** questions. Give it a short name; questions in the same category/unit with distinct values (≥ 12% apart) can be grouped together. Questions without a label still work as Estimate, Multiple choice and Higher/lower.
