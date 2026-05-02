# Sequel Marketing in Cinema: A Data Analysis

> **605 movies. Decades of franchises. One question: when does the sequel actually pay off?**

![Hero](images/analysis_plot_1.png)

![Python](https://img.shields.io/badge/python-3.x-blue) ![Notebook](https://img.shields.io/badge/jupyter-notebook-orange) ![Type](https://img.shields.io/badge/type-research--paper-purple)

---

## About

**Who:** Gyanesh Samanta — solo author, written as a research paper.
**What:** A data-driven study of franchise economics in cinema — comparing originals vs. sequels across budget, lifetime gross, ROI, and genre moats.
**When:** Authored February 2026.
**Where:** Jupyter notebook + accompanying paper, using a curated `MovieFranchises.csv` dataset of **605 movies** across major studios and franchises.
**Why:** Hollywood has bet hard on franchises for two decades. This paper examines whether the bet is still paying off — and which franchise traits separate the winners from the burnouts.

## The Story

The dataset spans **605 movies**, **13 fields** per movie (lifetime gross, budget, year, studio, rating, runtime, vote average, franchise ID, and more), going back to *Star Wars: A New Hope* (1977, $11M budget, $775M gross).

The analysis answers four questions:

1. **Does more budget mean more gross?** Yes — but with diminishing returns. Past a certain budget threshold, sequels show meaningfully lower marginal ROI than their originals.
2. **Which franchises set the ceiling?** Star Wars and the MCU (Avengers arc) dominate the lifetime-gross leaderboard, defining the benchmark every other franchise is measured against.
3. **Are franchise ROIs declining?** Yes. Rising production and marketing costs have compressed ROI on modern installments even as gross headlines grow.
4. **What makes a "moat"?** Action and Adventure genres carry most successful franchises, with PG/PG-13 ratings dominating the high-gross tier.

The paper contributes a working framework for evaluating sequel marketing decisions: **budget tier × genre × installment number** is a stronger predictor of ROI than star power alone.

## Gallery

| Budget vs. Gross | Top Franchises |
|---|---|
| ![Plot 0](images/analysis_plot_0.png) | ![Plot 1](images/analysis_plot_1.png) |

| ROI Over Time | Genre Moats |
|---|---|
| ![Plot 2](images/analysis_plot_2.png) | ![Plot 6](images/analysis_plot_6.png) |

Additional plots (`analysis_plot_3` through `analysis_plot_8`) cover studio splits, rating distributions, and runtime trends.

---

## Tech Stack

- **Python 3.x** — language
- **pandas / NumPy** — data wrangling
- **Matplotlib / Seaborn** — visualization
- **Jupyter Notebook** — analysis environment

## Repo Structure

```
Sequel-Marketing-in-Cinema-Analysis/
├── Cinematic_Franchise_Analysis.ipynb   # Full notebook
├── MovieFranchises.csv                  # 605 movies, 13 columns
├── images/                              # 9 generated plots
└── README.md
```

## Getting Started

```bash
git clone https://github.com/GyaneshSamanta/Sequel-Marketing-in-Cinema-Analysis.git
cd Sequel-Marketing-in-Cinema-Analysis
pip install pandas numpy matplotlib seaborn jupyter
jupyter notebook Cinematic_Franchise_Analysis.ipynb
```

Run all cells top-to-bottom; plots render inline and are also saved to `images/`.

## Contributing

This is a research artifact, but extensions welcome — particularly:

- Sentiment analysis correlating marketing hype with opening-weekend gross
- Predictive modeling (Random Forest / XGBoost) for "success" classification
- A "star power" index from cast metadata

## License

Released for academic and educational use.

## Credits

Authored by **Gyanesh Samanta** ([@GyaneshSamanta](https://github.com/GyaneshSamanta)). Dataset compiled from public box-office and franchise databases.
