# Course Recommendation System

A Recommendation System project that recommends similar Udemy courses using simple NLP and cosine similarity.

## Overview
- Uses course titles (cleaned) vectorized with `CountVectorizer`.
- Computes cosine similarity to recommend courses similar to a selected title.
- Implemented as a Jupyter Notebook: `course-recommendation-system.ipynb`.

## Files
- `course-recommendation-system.ipynb` — main notebook with preprocessing, vectorization, and recommendation code.
- `udemy_course_data.csv` — dataset (CSV of Udemy courses).
- `requirements.txt` — Python package requirements.

## Setup
1. Create a virtual environment (recommended):

   - On Windows (PowerShell):

     ```powershell
     python -m venv .venv
     .\.venv\Scripts\Activate.ps1
     ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Open the notebook in Jupyter and run cells:

   ```bash
   jupyter notebook course-recommendation-system.ipynb
   ```

## Notes
- The notebook contains a line that reads the CSV from a Kaggle input path: `/kaggle/input/course-recommendation-system-dataset/udemy_course_data.csv`.
- If you run locally, update the CSV path in the notebook to `udemy_course_data.csv` or the appropriate local path before running.
- The notebook uses `neattext` for basic text cleaning. If you prefer, you can replace those calls with `nltk` or `spaCy` equivalents.

## Usage
- Run the notebook, set a course title, and the notebook will output similar courses with similarity scores and metadata (URL, price, subscribers).

---
