## Tutorials for Mechanical Engineering Students

A hands-on introduction to machine learning for mechanical engineering students.
These notebooks cover foundational ML concepts, failure analysis, and time-series
analysis for remaining useful life (RUL) prediction — all in the context of
machine health monitoring.

The notebooks are numbered and should be followed in order:

| Notebook | Topic |
|---|---|
| `tut0_ml_foundations.ipynb` | Core ML concepts: bias-variance, overfitting, regularisation, cross-validation |
| `tut1_failure_analysis.ipynb` | Failure classification using sensor data (AI4I 2020 dataset) |
| `tut2_rul_timeseries.ipynb` | RUL prediction from time-series sensor data (NASA CMAPSS dataset) |

You are encouraged to experiment within each notebook.

### Setup

Requires Python 3.9+. We recommend [Miniconda](https://docs.anaconda.com/miniconda/).

**Create and activate an environment:**
```shell
conda create -n mech-ml python=3.11 -y
conda activate mech-ml
```

**Install dependencies:**
```shell
pip install numpy pandas matplotlib seaborn scipy \
            scikit-learn xgboost \
            jupyter notebook ipykernel
```

**Register the environment as a Jupyter kernel:**
```shell
python -m ipykernel install --user --name mech-ml --display-name "Python (mech-ml)"
```

**Launch Jupyter:**
```shell
jupyter notebook
```

Once Jupyter opens in your browser, open a notebook and select
**Kernel → Change kernel → Python (mech-ml)** before running any cells.

**Verify your installation** by running this in any notebook cell:
```python
import numpy, pandas, matplotlib, seaborn, scipy, sklearn
print("All good.")
```

No GPU is required. All notebooks run on a standard laptop with 4 GB RAM.

### Queries

For any issues or questions, please contact
[Tirtharaj Dash](mailto:tirtharaj@goa.bits-pilani.ac.in),
[MAHI Lab](https://mahi-group.github.io), Department of CS & IS, BITS Pilani Goa Campus.

Additional reading references are included at the end of each notebook.
