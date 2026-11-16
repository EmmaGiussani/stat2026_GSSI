# Statistica 2026 - GSSI

Repository degli esercizi del corso di statistica al GSSI, svolti in notebook
Python.

## Ambiente

Le dipendenze del progetto sono definite in `pyproject.toml` e `uv.lock`.
Dalla cartella della repository, sincronizza l'ambiente con:

```bash
uv sync
```

Per avviare JupyterLab:

```bash
uv run jupyter lab
```

In VS Code, seleziona come kernel l'interprete Python della cartella `.venv`.

## Esercizi

I notebook saranno raccolti nella cartella `esercizi/` e nominati, per esempio,
`es01_argomento.ipynb`. Le spiegazioni vanno inserite in celle Markdown e le
formule possono essere scritte in LaTeX.
