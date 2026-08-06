# Sleep, Doomscrolling & Digital Wellbeing

A portfolio-ready exploratory analysis of 1,000 respondents examining the relationships between bedtime screen habits, doomscrolling, sleep duration, sleep latency, weekly sleep debt, stress, and daytime fatigue.

## Project highlights

- Audits dataset grain, missingness, duplicates, ranges, and category balance.
- Compares doomscroller and non-doomscroller sleep outcomes.
- Explores sleep-quality segments and respondent-level relationships.
- Uses six GitHub-rendered visualizations with accessible labels and honest scales.
- Builds a leakage-controlled random-forest benchmark for sleep-quality classification.
- Separates observed associations from causal conclusions.

## Key findings

- 47.6% of respondents are labelled doomscrollers.
- Doomscrollers average 33.4 minutes of sleep latency versus 22.9 minutes for non-doomscrollers.
- Doomscrollers average 0.24 fewer sleep hours per night and 1.49 more weekly sleep-debt hours.
- Bedtime screen time correlates with nightly sleep duration at -0.44.
- The predictive benchmark reaches 58.0% test accuracy versus a 34.0% majority-class baseline.

These findings are observational associations and do not establish causality.

## Repository structure

```text
Sleep_Doomscrolling_Analysis/
├── data/
│   └── sleep_doomscrolling_habits.csv
├── sleep_doomscrolling_analysis.ipynb
├── requirements.txt
└── README.md
```

## Run locally

```bash
python -m venv .venv
```

Activate the environment, then install dependencies:

```bash
pip install -r requirements.txt
jupyter lab
```

Open `sleep_doomscrolling_analysis.ipynb` and run all cells from top to bottom. The notebook uses a relative data path, so it works after cloning without edits.

## Validation status

- Notebook schema validated with `nbformat`.
- All 12 code cells executed successfully in order.
- Zero unexecuted code cells and zero error outputs.
- Six embedded charts visually inspected.
- Source CSV contains 1,000 unique respondent IDs and no duplicate rows.

## Limitations

The supplied archive does not include collection methodology, sampling design, survey date, field definitions, or license metadata. Some fields contain 2–5% missing values. Treat the model as a reproducible portfolio benchmark, not a clinical or diagnostic tool.
