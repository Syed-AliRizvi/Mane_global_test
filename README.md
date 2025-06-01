# Mane Global Test

This repository contains code and answers for the Mane Global data engineering test.

---

## Project Structure
```
Mane_global_test/
├── q1_solution_time_series_analysis/
│ ├── input_data/                               # Contains quarter_dates.csv and daily_data.csv
│ ├── output_data/                              # Contains the generated quarterly_data.csv
│ └── scripts/                                  # Jupyter notebook (mane_global_test_20250601.ipynb) for Section 1
├── q2_solution_vue_app/
│ └── index.html                                # Vue static page displaying the quarterly table
├── q3_solution_de_questions/
|  └── section2_answers.docx                    # Written answers for Section 2
├── .gitignore
├── requirements.txt
├── Mane Global Capital Management Test.docx    # Questions for Mane Global CM. 
└── README.md                                   # Project documentation
```

---

## Setup Instructions

Clone the Repository
```
git clone https://github.com/Syed-AliRizvi/Mane_global_test.git
cd Mane_global_test
```
---

## View Section 1 (Time series analysis)

### 1. Create a Virtual Environment (optional but recommended)

- Mac/Linux:
    ```
    python3 -m venv timeseries_env
    source timeseries_env/bin/activate
    ```
- Windows (PowerShell):
    ```
    python -m venv timeseries_env
    .\timeseries_env\Scripts\Activate.ps1
    ```

### 2. Install Dependencies
```
pip install --upgrade pip
pip install -r requirements.txt
```
if you want to use the virtual environment as a jupyter notebook kernel run the following
```
pip install jupyterlab ipykernel
python -m ipykernel install --user --name=timeseries_env --display-name "Python (timeseries_env)"
```

### 3. Launch Jupyter Notebook

```
jupyter lab 
```
or 
```
jupyter notebook
```
- Open `q1_answer/scripts/test.ipynb` in Jupyter and run all cells.

---

## View Section 2 (Vue static page)
```
python -m http.server 8000
```
- In your browser, go to:  `http://localhost:8000/q2_answer/index.html`

---

## Section 3 (Written answers)
- Open `q3_answer/section2_answers.docx` in any word processor.

## Deactivate the virtual environment when done**
```
deactivate
```

---

## Notes

- Make sure your Python version is 3.8 or above.
- Data files are in `q1_solution_time_series_analysis/input_data/`.
- Output files will be saved in `q1_solution_time_series_analysis/output_data/`.
- If you add or change dependencies, update `requirements.txt` with `pip freeze > requirements.txt`.


---
