# Statistics 2026 - GSSI

Exercises and lecture notes for the statistics course at GSSI. Exercises are
solved in Python notebooks; the lecture notes are collected in a single PDF.

## Repository layout

```
exercises/
  01_distributions/        one folder per course topic
    ex01_<name>.ipynb      one notebook per exercise (numbering restarts in each topic)
  02_monte_carlo/
notes/
  lecture_notes.pdf        reviewed lecture notes (single file, updated in place)
```

The exercise texts are the Markdown cells at the top of each notebook. The
lecture notes PDF points to the notebook where each exercise is solved.

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
