# Assignment A2 — Proof of Life
* **Repository Target Grade:** 20 Marks (Course Rubric)
* **Student Registration Number:** 24/2319/BSCE-S

## Program Description
This repository contains a structured data pipeline built in Google Colab. The application automates loading a regional housing dataset, handles missing structural values cleanly, and prepares raw inputs for subsequent engineering evaluations.

## File List
* `README.md` - Assignment documentation and system run guide.
* `CML3112_24_2319_BSCE_S_W02.ipynb` - The primary verified execution notebook.
* `california_housing_train.csv` - The source dataset containing regional survey details.

## Run Instructions
1. Open the notebook file `CML3112_24_2319_BSCE_S_W02.ipynb` in Google Colab.
2. Ensure the standard workspace environment contains `california_housing_train.csv`.
3. Select **Runtime -> Restart session and run all** from the top controls.

## Engineering Problem Included
* **Problem:** Raw numerical tables frequently feature empty entries or unformatted decimals which disrupt exact statistical counts.
* **Solution:** Automated missing value cleanup with zero-fills and standard typecasting (`.fillna(0).astype(int)`).

## Error Log Record
* **Error Encountered:** `NameError: name 'csv_filename' is not defined`
* **Repair Action:** Explicitly declared the missing string file path variable at the start of the data loading block.
