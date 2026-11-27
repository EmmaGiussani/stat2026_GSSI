# Statistics 2026 - GSSI

Lecture notes and exercises for the statistics course at GSSI, all written as
Python notebooks: one notebook per topic, one notebook per exercise.

## Repository layout

```
lectures/
  L01_probability.ipynb               one notebook per course topic,
  L02_distributions.ipynb             with figures already executed
  L03_monte_carlo.ipynb               (the banner gives the lecture and date)
  L04_information_measurement.ipynb
  L05_point_estimation.ipynb
exercises/
  01_distributions/        one folder per course topic
    ex01_<name>.ipynb      one notebook per exercise (numbering restarts in each topic)
  02_monte_carlo/
  03_point_estimation/
  04_interval_estimation/
```

Each lecture notebook links to the exercises of that lecture. The exercise
texts are the Markdown cells at the top of each exercise notebook, followed by
the solution.

## Credits

The lectures are by G. Benato (GSSI). A few examples in the lecture notebooks
are inspired by D. Gerosa's
[Astrostatistics and Machine Learning](https://github.com/dgerosa/astrostatistics_bicocca_2025)
(Milano-Bicocca 2025).

## Environment

Dependencies are defined in `pyproject.toml` and `uv.lock` (managed with
[uv](https://docs.astral.sh/uv/)). From the repository folder:

```bash
uv sync                # create/update .venv
uv run jupyter lab     # start JupyterLab
```

In VS Code, select the interpreter in `.venv` as the notebook kernel.
Add new libraries with `uv add <package>`, never with `pip install`.

## Conventions

- Everything in the repository (notebooks, notes, commit messages) is in English.
- Notebook names: `exNN_<topic>.ipynb`, inside the folder of the topic.
- Explanations go in Markdown cells, formulas in LaTeX.
- Before each commit: *Restart Kernel and Run All*, so the notebook is known to
  run from top to bottom.
