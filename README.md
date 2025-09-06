# Project Portfolio Analysis

## Overview

This repository contains a self‑contained data project designed to showcase skills relevant for business analysts, program managers, and data analysts. The project uses a synthetic dataset representing a portfolio of 200 projects, with attributes such as budgets, durations, team sizes, complexity levels, risk assessments, and satisfaction scores. The accompanying notebook demonstrates how to load the data, perform exploratory data analysis (EDA) with visualizations, and build predictive models.

The goal is to provide a ready‑to‑use example that you can clone, run locally, and extend. It illustrates proficiency in data wrangling, visualization, and machine learning while telling a clear story about project performance and outcomes.

## Repository Structure

```
├── project_portfolio_data.csv         # Synthetic dataset (200 rows)
├── project_portfolio_analysis.ipynb   # Jupyter Notebook with EDA and models
├── requirements.txt                   # Python dependencies
└── README.md                          # Project documentation (this file)
```

## Dataset Description

Each row in `project_portfolio_data.csv` represents a single project. Columns include:

| Column                     | Type/Unit | Description |
|----------------------------|-----------|-------------|
| **Project_ID**             | integer   | Unique identifier for the project |
| **Project_Name**           | string    | Project name (e.g., “Project 1”) |
| **Start_Date**             | date      | Start date of the project |
| **Planned_End_Date**       | date      | Planned completion date |
| **Actual_End_Date**        | date      | Actual completion date |
| **Planned_Duration_Days**  | integer   | Planned duration in days |
| **Actual_Duration_Days**   | integer   | Actual duration in days |
| **Planned_Budget**         | USD       | Planned budget (50k–500k) |
| **Actual_Budget**          | USD       | Actual spend |
| **Team_Size**              | integer   | Number of team members |
| **Complexity**             | category  | Project complexity (`Low`, `Medium`, `High`) |
| **Client_Satisfaction_Score** | float | Client satisfaction rating (1–10) |
| **Risk_Level**             | category  | Risk level (`Low`, `Medium`, `High`) |
| **Manager_Experience_Years** | integer | Years of experience for the program manager |
| **Completed**              | binary    | 1 if project completed before 2024-01-01, else 0 |

## Getting Started

### Prerequisites

- Python 3.8 or higher
- A working installation of Jupyter Notebook or JupyterLab

### Setup

1. **Clone the repository**

```bash
git clone https://github.com/<YOUR_USERNAME>/<REPO_NAME>.git
cd <REPO_NAME>
```

2. **Create and activate a virtual environment (optional but recommended)**

```bash
python -m venv .venv
source .venv/bin/activate  # On Windows use `.venv\Scripts\activate`
```

3. **Install the required packages**

```bash
pip install -r requirements.txt
```

4. **Launch the notebook**

```bash
jupyter notebook project_portfolio_analysis.ipynb
```

Follow the steps in the notebook to explore the data, visualize relationships, and build predictive models. Feel free to modify the code, adjust model parameters, or add new analyses to deepen your insights.

## Extending the Project

The synthetic dataset and notebook are intended as a starting point. You can extend this project by:

- **Hyperparameter tuning**: Experiment with different algorithms (e.g., gradient boosting, XGBoost) and optimize parameters.
- **Feature engineering**: Create new variables (e.g., budget overrun percentage, schedule variance) to improve predictive power.
- **Dashboarding**: Build interactive dashboards using libraries like Plotly Dash or Streamlit to present findings.
- **Real data integration**: Replace the synthetic dataset with real project management data (if available) to generate actionable insights.

## License

This project is provided under the MIT License. See the `LICENSE` file for details.
