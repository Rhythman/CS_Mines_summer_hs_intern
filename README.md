# CS@Mines Summer Internship - High School Track

Welcome! 👋 This repository holds the hands-on materials for the CS@Mines summer internship.
Each day pairs a short lecture with time to build things yourself.
You already know some Python - here you will learn the tools and ideas that working data scientists and engineers use every day.

## What this is

A small, friendly set of notebooks and guides.
Day 1 gets you comfortable in Jupyter and walks you through your very first machine learning (ML) workflow.
Day 2 (coming soon) moves on to Transformers, large language models (LLMs), and building your own website.

You do not need to install anything to get started - every notebook has a one-click **Open in Colab** button below that runs in your browser.

## Repository map

```
CS_Mines_summer_hs_intern/
├── README.md                  ← you are here
├── requirements.txt           ← packages to install if you run locally
└── day1/
    ├── README.md              ← Day 1 guide: schedule + how to use the notebooks
    ├── notebooks/             ← the notebooks you work in
    │   ├── 01_demo_intro_to_jupyter_and_ml.ipynb
    │   └── 02_titanic_practice_template.ipynb
    ├── solutions/             ← the answer key (peek only when you are stuck!)
    └── data/                  ← the Titanic dataset, bundled so nothing to download
```

## Day 1 - Intro to Jupyter & Machine Learning

Two Jupyter notebooks. Do them in order.

| # | Notebook | What it is | Open in Colab |
|---|----------|------------|---------------|
| 1 | [`01_demo_intro_to_jupyter_and_ml.ipynb`](day1/notebooks/01_demo_intro_to_jupyter_and_ml.ipynb) | A guided **demo**: learn how Jupyter works, then watch one short ML workflow end to end. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Rhythman/CS_Mines_summer_hs_intern/blob/main/day1/notebooks/01_demo_intro_to_jupyter_and_ml.ipynb) |
| 2 | [`02_titanic_practice_template.ipynb`](day1/notebooks/02_titanic_practice_template.ipynb) | A **fill-in-the-blank** project where you build a Titanic survival model yourself. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Rhythman/CS_Mines_summer_hs_intern/blob/main/day1/notebooks/02_titanic_practice_template.ipynb) |

Stuck on the practice notebook? The complete worked answer key lives in [`day1/solutions/`](day1/solutions/).
Try each step yourself first - that is where the learning happens.

See the [**Day 1 guide**](day1/README.md) for the schedule and step-by-step instructions.

## Day 2 - Coming soon

> 🚧 **Coming soon:** Transformers, LLMs & building your own website. Check back after Day 1.

## How to open the notebooks

You have two options. Pick whichever is easier for you.

### Option A - Google Colab (easiest, nothing to install)

Click an **Open in Colab** badge above.
It opens the notebook in your browser with everything already set up.
If Colab asks, sign in with a Google account. That is it.

### Option B - Run locally on your own computer

If you would rather run things on your own machine:

```bash
# 1. Download the repository
git clone https://github.com/Rhythman/CS_Mines_summer_hs_intern.git
cd CS_Mines_summer_hs_intern

# 2. Install the required packages
pip install -r requirements.txt

# 3. Launch Jupyter and open a notebook from the day1/notebooks/ folder
jupyter notebook
```

A virtual environment is optional but recommended if you know how to make one.

## About the data

The Titanic dataset is already **bundled in [`day1/data/`](day1/data/)**, so you do not have to download anything.
The notebooks load it automatically whether you are on Colab or running locally.

## If a notebook starts acting weird

Cells remember everything you have run, so out-of-order runs can confuse things.
When in doubt, reset and start fresh:

> 💡 **Tip:** use **Kernel → Restart & Run All** (in Colab it is **Runtime → Restart and run all**).
> This clears everything and re-runs the notebook cleanly from the top. It fixes most "why is this broken?" moments.

Happy building! 🚀
