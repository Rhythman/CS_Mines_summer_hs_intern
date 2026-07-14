# Day 1: Intro to Jupyter & Machine Learning

Today you will get comfortable working in Jupyter and build your very first machine learning (ML) model: a program that predicts which Titanic passengers survived.
No prior ML experience needed. You just need the Python you already know.

## The plan for today

| When | What | Roughly |
|------|------|---------|
| Morning | Lecture on ML concepts: what ML is, features vs. labels, training vs. testing, overfitting, and how models are scored. | ~2 hours |
| Rest of day | Self-practice with the two notebooks below. Work at your own pace. | ~5 hours |

The lecture teaches the **ideas**. The notebooks teach the **hands-on skills** and let you apply those ideas in code.
You do not need to memorize anything from the lecture. The notebooks remind you of each concept as it comes up.

## The two notebooks (do them in order)

Both live in [`notebooks/`](notebooks/). Open each with the **Open in Colab** badge in the [main README](../README.md), or run them locally.

### 1. Demo first: learn the tool

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Rhythman/CS_Mines_summer_hs_intern/blob/main/day1/notebooks/01_demo_intro_to_jupyter_and_ml.ipynb)

Open [`01_demo_intro_to_jupyter_and_ml.ipynb`](notebooks/01_demo_intro_to_jupyter_and_ml.ipynb) and **read + run every cell in order**.

This notebook shows you:

- How Jupyter works: cells, the kernel, running code with Shift+Enter, and how notebooks remember state.
- How to read errors and recover from a confused notebook.
- One short ML workflow from start to finish, so you see the shape of what you are about to build.

Do not skip this one. It is where you learn the tool you will use for the rest of the day.

### 2. Practice second: build it yourself

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Rhythman/CS_Mines_summer_hs_intern/blob/main/day1/notebooks/02_titanic_practice.ipynb)

Open [`02_titanic_practice.ipynb`](notebooks/02_titanic_practice.ipynb) and work through it.

This is a fill-in-the-blank notebook. As you go, you will:

- Find spots marked **TODO** where some code is left blank for you to complete.
- Fill in the missing code, then run the cell.
- Run the **Self-check** cell right after each TODO. It tells you whether your answer looks right and prints the value to expect.

The blanks start easy and get bigger on purpose as you build confidence.
Read the markdown notes and study every figure. Each one is explained.

## Where the answer key is

The full worked solution lives in [`solutions/`](solutions/).

Use it as a safety net, not a shortcut:

- Try every TODO yourself first, and use the hints inside the notebook before peeking.
- If you get truly stuck on a step, check that one step in the solution, then come back and keep going.

## Tips for a smooth day

- Run cells in order, top to bottom. Notebooks remember everything you have run, so jumping around causes confusing bugs.
- If things get weird, reset. Use **Kernel → Restart & Run All** (Colab: **Runtime → Restart and run all**) to re-run cleanly from the top. This fixes most problems.
- Read the error, don't fear it. Errors are normal. Read the last line of the message first, since it usually says exactly what went wrong.
- The data is already included. The Titanic files are bundled in [`data/`](data/), so the notebooks load them for you with no download.
- Go at your own pace. There is no rush. Understanding one step well beats rushing through five.

Have fun, and don't be afraid to experiment! 🚢
