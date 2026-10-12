# Week 1 presentation · Tuesday 13 October 2026

Each of you gets a **unique real-world dataset and business problem**. It's on your **W1 card on Trello**. Your job is to solve it with machine learning and present it.

**10 minutes per person**:

| Part | Time |
|---|---|
| Slides: the business problem and your solution | ~4 min |
| Notebook walkthrough: what you did and what you found | ~4 min |
| Questions | ~2 min |

> Your problem statement deliberately does **not** say whether it's classification or regression. Working that out, and explaining why, is part of the task.

---

## What to prepare

### 1. Jupyter notebook

Follow this structure, with a markdown heading for each section:

| # | Section | What to show |
|---|---|---|
| 1 | **Problem and data** | The business problem in your own words; load the data; `shape`, `head()`, `info()` |
| 2 | **Data cleaning** | Missing values, duplicates, outliers, wrong data types, and what you did about each one, and why |
| 3 | **Data visualisation** | The target variable's distribution; how the key features relate to the target; a correlation heatmap; 3-5 charts, each with a one-line takeaway |
| 4 | **Data preprocessing** | Imputation, encoding, scaling, and the train/test split (split **before** fitting scalers or imputers) |
| 5 | **Problem type** | Classification or regression, and why |
| 6 | **Model comparison** | Train **at least 3** algorithms from Week 1 on the same split. Show one results table with the right metrics: train **and** test scores |
| 7 | **Best algorithm and why** | Pick one and justify it: test performance, generalisation (gap between train and test), interpretability, speed. Tune it if you have time (cross-validation, grid search) |
| 8 | **Conclusion** | What the model means for the business, its limitations, and what you'd do next |

**Metrics reminder**
- **Regression:** MAE, RMSE, R²
- **Classification:** accuracy, precision, recall, F1, ROC-AUC, confusion matrix. Say which matters most for **your** business problem, and why.

### 2. Slide deck (about 5 slides)

Aim it at a **business audience**: light on code, heavy on the "so what".

| Slide | Content |
|---|---|
| 1 | **The business problem.** Who has it, why it matters, what it costs |
| 2 | **The data.** Where it's from, size, key features, data-quality issues found |
| 3 | **The approach.** How ML solves it: problem type, models compared, how you evaluated them |
| 4 | **Results.** The comparison and the best model, with one clear chart or table |
| 5 | **Recommendation and next steps.** How the business should use it, risks and limitations, what to do next |

Use PowerPoint, Google Slides or Canva, and export to PDF.

---

## How to submit

On your fork of this repo, on your branch `week1/<your-name>`:

```
presentation/
├── README.md       # your problem statement + a link to the dataset
├── analysis.ipynb  # the notebook, run top to bottom with outputs saved
└── slides.pdf      # the deck
```

- **Don't commit the dataset itself** if it's large. Link to it in your README instead.
- `git add .`, `git commit -m "Add Week 1 presentation"`, `git push`
- **By the end of Monday 12 Oct** (prep day): post the link to your branch as a comment on your W1 Trello card, then move the card to **Review**.

## Checklist

- [ ] The notebook runs top to bottom without errors
- [ ] Cleaning, visualisation and preprocessing each explain **why**, not just what
- [ ] At least 3 algorithms compared in one table, with train and test scores
- [ ] Problem type stated and justified
- [ ] Best algorithm chosen, with reasons
- [ ] About 5 slides that a non-technical manager could follow
- [ ] Rehearsed to fit in 10 minutes, including questions
- [ ] Pushed to GitHub, with the link on your Trello card
