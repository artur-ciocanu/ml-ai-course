# Local setup
The setup uses VS Code's Jupyter extension for [assignment.ipynb](assignment.ipynb) and `uv` to manage the Python environment.

## Environment files
- `pyproject.toml` - lists the packages and requires Python 3.14 or newer.
- `uv.lock` - keeps package versions consistent across setups.
- `.venv/` - holds the local Python environment and is excluded from Git.

## Run in VS Code
1. Install [uv](https://docs.astral.sh/uv/) and the Python and Jupyter extensions for VS Code.
2. Open `module-5-application` in VS Code. In its terminal, run:
   ```sh
   uv sync --locked
   ```
3. Open `assignment.ipynb` and select `.venv` under **Select Kernel**.
4. Restart the kernel, run all cells, and save the notebook with its results and plots.

## Use JupyterLab instead
Run this from `module-5-application`:
```sh
uv run jupyter lab
```

Open `assignment.ipynb` and use the project's Python environment.

Keep `data/coupons.csv` unchanged - use `cleaned_data` for the cleaning and analysis.
