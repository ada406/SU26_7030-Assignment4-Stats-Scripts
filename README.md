# Assignment 4 – Stats Scripts

Repository: [SU26_7030-Assignment4-Stats-Scripts](https://github.com/ada406/SU26_7030-Assignment4-Stats-Scripts)

SciPy statistics tutorial work for BSGP 7030.

## Structure

- `manual/` – hand-written tutorial notebook and data
- `ai/` – AI-assisted version

## OSC OnDemand quick start

```bash
cd ~/SU26_7030-Assignment4-Stats-Scripts
ls manual ai
cd ai   # or: cd manual
ls environment.yml stats_python.ipynb brain_size.csv
module load miniconda3
conda env create -f environment.yml   # first time only
conda activate stats-env
```

Then open the notebook in Jupyter from that same folder.
