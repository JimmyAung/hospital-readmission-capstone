# Hospital Readmission Capstone

A machine learning project focused on predicting 30-day hospital readmissions with an emphasis on recall optimization.

## Overview

This capstone project implements a recall-first approach to predict whether a patient will be readmitted to the hospital within 30 days of discharge. The project emphasizes identifying as many at-risk patients as possible (high recall) to enable proactive intervention, even if it means accepting more false positives.

**Key Features:**
- Exploratory Data Analysis (EDA) and feature engineering
- Multiple ML models: Logistic Regression and Random Forest
- Decision threshold tuning for recall optimization
- Interactive Power BI dashboard for insights visualization
- Reproducible workflow with detailed documentation

## Repo Structure

```
hospital-readmission-capstone/
├── data/                    # Data directory (raw data excluded from repo)
│   └── README.md           # Instructions for accessing the dataset
├── notebooks/              # Jupyter notebooks for analysis and modeling
│   ├── 01_eda.ipynb       # Exploratory data analysis
│   ├── 02_preprocessing.ipynb  # Data cleaning and feature engineering
│   └── 03_modeling.ipynb  # Model training and evaluation
├── dashboard/              # Power BI dashboard files
│   └── readmissions.pbix  # Interactive visualization dashboard
├── LICENSE                 # Project license
└── README.md              # This file
```

## Data Access

The raw dataset is not included in this repository due to size and privacy considerations. To reproduce this analysis:

1. Refer to `/data/README.md` for detailed instructions on obtaining the dataset
2. Download the data following the provided guidelines
3. Place the data files in the `data/` directory as specified

## Notebooks

The analysis is organized into sequential Jupyter notebooks:

1. **EDA Notebook** (`01_eda.ipynb`): Initial data exploration, visualization of patient characteristics, and identification of patterns related to readmission
2. **Preprocessing Notebook** (`02_preprocessing.ipynb`): Data cleaning, handling missing values, feature engineering, and preparation for modeling
3. **Modeling Notebook** (`03_modeling.ipynb`): Model training (Logistic Regression, Random Forest), hyperparameter tuning, and threshold optimization for recall

Each notebook includes detailed markdown explanations and is designed to be run sequentially.

## Power BI

An interactive Power BI dashboard (`dashboard/readmissions.pbix`) provides visual insights into:
- Patient demographics and readmission patterns
- Feature importance and model performance metrics
- Threshold impact analysis
- Risk stratification visualizations

To view the dashboard, open the `.pbix` file using Power BI Desktop (available for free from Microsoft).

## Quick Start

1. **Clone the repository:**
   ```bash
   git clone https://github.com/JimmyAung/hospital-readmission-capstone.git
   cd hospital-readmission-capstone
   ```

2. **Set up your environment:**
   ```bash
   # Create a virtual environment
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   
   # Install dependencies
   pip install -r requirements.txt  # If requirements file is provided
   ```

3. **Obtain the data:**
   - Follow instructions in `data/README.md` to download the dataset
   - Place data files in the `data/` directory

4. **Run the notebooks:**
   ```bash
   jupyter notebook
   ```
   - Execute notebooks in sequence: `01_eda.ipynb` → `02_preprocessing.ipynb` → `03_modeling.ipynb`

5. **Explore the dashboard:**
   - Open `dashboard/readmissions.pbix` in Power BI Desktop

## License

This project is licensed under the terms specified in the [LICENSE](LICENSE) file.
