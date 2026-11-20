# HCL-Training-Source-code
source Code
# Student Academic Performance Analytics — Project 2

## Files
- `02_student_performance.csv` — input dataset
- `student_performance_analysis.py` — pandas/NumPy analysis source code
- `Student_Academic_Performance_Analytics_Report.docx` — analysis report
- `Student_Academic_Performance_SRS.docx` — Software Requirements Specification

## Requirements
```bash
pip install pandas numpy
```

## Run
Place the CSV and Python file in the same folder, then run:
```bash
python student_performance_analysis.py
```

The script exports cleaned data and summary CSV files into the current folder.

## Analysis rules
- Missing attendance values are filled with the median.
- Total and average marks use Python, Maths and Physics.
- Grade bands: A (90–100), B (80–<90), C (70–<80), D (60–<70), F (<60).
- At-risk threshold: average marks below 40.
- Python mark outliers: 1.5 × IQR rule.
