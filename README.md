# DataFix AI — Autonomous Data Quality & Repair Engine

## Features
- Upload CSV and Excel files
- Detect missing values, exact duplicates, text whitespace/case inconsistencies and numerical IQR outliers
- Repair missing numeric values with median and categorical values with mode
- Trim whitespace and cautiously normalize low-cardinality text
- Remove exact duplicate rows
- Display before/after quality scores and remaining issues
- Download cleaned CSV and audit log

## Setup
1. Install Python 3.10+.
2. Open this folder in VS Code.
3. In a terminal, create a virtual environment:
   - Windows: `py -m venv .venv` then `.venv\\Scripts\\activate`
   - macOS/Linux: `python3 -m venv .venv` then `source .venv/bin/activate`
4. Install: `pip install -r requirements.txt`
5. Launch: `streamlit run app.py`
6. Upload a CSV/Excel file, or click **Load sample dataset**, then click **Run DataFix repair**.

Outliers are flagged but not automatically changed. Review repair logs before relying on cleaned data.
