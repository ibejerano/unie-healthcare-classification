# diabetes_multiclass_classifier

**Academic, reproducible pipeline** for multiclass diabetes status classification (No/Prediabetes/Diabetes) using BRFSS 2015 Diabetes Health Indicators dataset (253K U.S. adults).

**Purpose**: End-to-end analysis emphasizing data quality assessment, leakage prevention, feature engineering, class imbalance handling, and supervised learning models to **predict diabetes status**. Achieves **macro AUC=0.76** with Random Forest diabetes recall=0.69, Gradient Boosting prediabetes recall=0.29. Formal hypothesis testing rejects H₀ (LR=36,304, p<0.0001), confirming hypertension OR=2.50 as strongest risk gradient. Interprets results under **associational framework**, quantifying self-reported survey data limitations absent clinical biomarkers.

## Project Structure
```bash
.
├── datasets/
│ └── diabetes_012_health_indicators_BRFSS2015.csv # CC BY 4.0 License (dataset)
├── src/ 
│ └── diabetes_multiclass_classifier.ipynb # Complete executable pipeline
├── requirements.txt
├── LICENSE # MIT License (code)
└── README.md
```

## Copyright and License

- **© 2026 Isabel Bejerano Blazquez**
- **Notebook**: MIT License
- **Data**: CC BY 4.0

eveloped and tested on:

- **Python ≥ 3.10**  
- **Core dependencies:** see requirements.txt file

## Quick start

```bash
## Create and activate environment
python3.10 -m venv venv
source venv/bin/activate      # macOS/Linux
venv\Scripts\activate         # Windows

# Install dependencies
pip install -r requirements.txt  

# Run notebook
jupyter notebook src/diabetes_multiclass_classifier
```

**Disclaimer**: Provided *as is*, for academic use only.