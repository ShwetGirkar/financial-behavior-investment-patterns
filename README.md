# Financial Behavior and Investment Patterns Survey

A reproducible semester-project analysis of survey responses about saving, investment awareness, financial confidence, and financial planning across self-selected age groups.

## Start here

1. Install Python 3.10 or later.
2. Create and activate a virtual environment.
3. Install dependencies: `pip install -r requirements.txt`.
4. Put a privacy-reviewed copy of the workbook at `data/survey_responses.xlsx`. The data directory is ignored by Git.
5. Start Jupyter with `jupyter notebook analysis.ipynb` and run all cells. Alternatively set `SURVEY_DATA_PATH` to a local workbook path.

The notebook removes timestamp, email, and name columns before analysis. It reports grouped summaries rather than individual responses. Review open-ended answers locally before any public release because free text can identify a respondent.

## Project contents

- `analysis.ipynb` — data cleaning, subgroup summaries, age-at-learning summaries, cross-tabulation, and charts.
- `results/analysis_summary.md` — findings calculated from the supplied workbook, with denominators and limitations.
- `results/figures/*.svg` — privacy-safe aggregate charts for the summary.
- `data/README.md` — instructions for keeping survey data local.
- `requirements.txt` — Python dependencies.

## Findings from the supplied workbook

The workbook contains 166 responses: 117 Youth, 4 Early Adult, 44 Midlife Adult, and 1 Senior. The sample is highly imbalanced; use the detailed summary for question-specific denominators and avoid generalizing the four Early Adult or one Senior responses.

## Privacy and GitHub

The original response workbook is not included. `.gitignore` excludes workbook, CSV, and data files by default. Before publishing, confirm consent and remove direct identifiers; review free-text responses for indirect identifiers too. To check locally before a first commit, run `git status --short` and confirm no response data is staged.

## Research limitations

Age bands are self-selected and the workbook labels overlap at age 50. The survey measures self-reported awareness and confidence rather than objective financial knowledge. Savings are categorical bands, and the study is cross-sectional, so associations do not establish causation.
