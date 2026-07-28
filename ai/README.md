# AI folder – Assignment 4 Stats Scripts

This folder is the AI-assisted version of the SciPy statistics tutorial exercises.

Tutorial: https://scipy-lectures.org/packages/statistics/index.html

## Files

| File | Purpose |
| --- | --- |
| `stats_python.ipynb` | Main notebook (brain size exercise answers) |
| `stats_extension.ipynb` | Extension: mixed-effects model on repeated IQ scores |
| `PROMPTS.md` | Log of prompts used to build the AI materials |
| `environment.yml` | Conda environment specification (`stats-env`) |
| `brain_size.csv` | Brain size / IQ dataset |
| `iris.csv` | Iris dataset |
| `wages.txt` | Wage dataset (from StatLib, linked in the tutorial) |

## Setup on OSC OnDemand

Open an OSC terminal and move into this folder:

```bash
cd ~/SU26_7030-Assignment4-Stats-Scripts/ai
ls environment.yml brain_size.csv stats_python.ipynb
```

If `ls` fails, you are in the wrong directory.

Load conda (module name may vary slightly on OSC), then create/activate the environment:

```bash
module load miniconda3
conda env create -f environment.yml
conda activate stats-env
```

If the environment already exists, skip `conda env create` and just run:

```bash
conda activate stats-env
```

## Run the notebook

1. Start **Jupyter** from OSC OnDemand.
2. Open `stats_python.ipynb` or `stats_extension.ipynb`.
3. Choose a kernel that uses the `stats-env` conda environment.
4. Run the notebook cells.

You can also check from the terminal:

```bash
cd ~/SU26_7030-Assignment4-Stats-Scripts/ai
conda activate stats-env
python -c "import pandas, numpy; print('OK')"
```

## Local Mac setup

Same commands, from this folder, if conda is already installed:

```bash
cd ~/SU26_7030-Assignment4-Stats-Scripts/ai
conda env create -f environment.yml
conda activate stats-env
jupyter lab
```
