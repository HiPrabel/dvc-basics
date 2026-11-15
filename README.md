# DVC Basic

A minimal machine learning project that demonstrates data versioning with DVC. The project trains a RandomForest regressor to predict wine quality from a CSV dataset.

## Project structure

- `train.py` - training script
- `utils.py` - helper functions for loading and preparing the dataset
- `requirements.txt` - Python dependencies
- `data/wine_sample.csv.dvc` - DVC metadata for the dataset

## Setup

1. Create and activate a virtual environment:

   ```bash
   python -m venv .venv
   source .venv/bin/activate
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. If the dataset is being managed by DVC, pull it before training:

   ```bash
   dvc pull
   ```

   If the CSV is already present locally, you can skip this step.

## Run training

```bash
python train.py --csv data/wine_sample.csv
```
