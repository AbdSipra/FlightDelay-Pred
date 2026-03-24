# Flight Delay Prediction

This project predicts flight delays by combining structured flight data extracted from Word documents with weather data stored in Excel files.

The notebook builds a preprocessing pipeline that reads raw `.docx` flight records, engineers features, merges weather information by date/time, performs exploratory analysis, and trains multiple prediction models.

## Problem Variants Covered

- Binary classification: delayed vs on-time
- Multi-class classification: delay severity categories
- Regression: predicted delay duration

## Workflow

- Extract structured fields from raw flight `.docx` files
- Preprocess monthly weather `.xlsx` files
- Merge flight and weather data
- Clean missing values and engineer features
- Explore delay patterns by hour, day, airline, and weather
- Train Random Forest models for different prediction targets
- Export submission-style CSV outputs

## Files

- `flight_delay_prediction.ipynb` - main notebook
- `Train/` - training flight documents
- `Test/` - test flight documents
- `Weather/` - weather spreadsheets

## Tech Stack

- Python
- Pandas
- NumPy
- python-docx
- openpyxl
- Scikit-learn
- Matplotlib
- Seaborn

## Important Note

The notebook contains hardcoded local paths in some cells. You should update those paths to match the folders inside this repository before running it.

## How to Run

1. Keep `Train`, `Test`, and `Weather` beside the notebook
2. Update any hardcoded file paths in the notebook
3. Install the required Python libraries
4. Run the notebook in order

## Summary

This repository is a notebook-based applied ML project that shows end-to-end data extraction, feature engineering, weather fusion, exploratory analysis, and predictive modeling from non-standard raw input formats.
