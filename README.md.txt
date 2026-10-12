NHS Emergency Care Intelligence: Performance Analysis and Demand Forecasting (2019–2026)

Project Overview

This project analyses seven years of NHS England Accident & Emergency (A&E) attendance and emergency admission data, covering April 2019 to March 2026.

The objective is to evaluate emergency care demand, investigate waiting-time performance, identify variations across NHS providers, and develop forecasting models to support evidence-based healthcare planning.

The project combines Python, statistical forecasting, and Power BI to transform publicly available NHS data into actionable insights.

Key Objectives

- Analyse historical A&E attendance and emergency admission trends.
- Evaluate NHS four-hour waiting-time performance.
- Investigate variations in emergency care performance across providers.
- Examine delays between the decision to admit and admission.
- Compare time-series forecasting models for predicting A&E demand.
- Develop interactive Power BI dashboards to communicate findings.

Tools and Technologies

- Python: Pandas, NumPy, data processing and exploratory analysis.
- Time-Series Forecasting: Holt-Winters, SARIMA and Seasonal Naive.
- Power BI: Data modelling, DAX measures and interactive dashboards.
- Jupyter Notebook: Reproducible data analysis and forecasting workflows.
- Data Source: NHS England A&E Attendances and Emergency Admissions monthly publications.


 Key Findings

The analysis covers 84 months of NHS England emergency care data, from April 2019 to March 2026.

Emergency Care Performance

- 168.96 million A&E attendances were recorded across the study period.
- 43.28 million emergency admissions were recorded.
- 22.61% was the overall four-hour waiting-time breach rate.
- 38.20 million attendances exceeded the four-hour waiting-time threshold.
- 9.10 million decision-to-admit waits exceeded four hours.
- The overall rate of decision-to-admit waits exceeding four hours was 5.39 per 100 A&E attendances.

These findings highlight the scale of emergency care demand and the importance of monitoring waiting-time performance and admission delays.

Forecasting Model Performance

Four forecasting approaches were evaluated against observed monthly A&E attendance figures for the 2025/26 financial year.

| Forecasting Model | MAPE |
|---|---:|
| Holt-Winters | 1.564% |
| Simplified SARIMA | 2.403% |
| Seasonal Naive | 2.405% |
| Original SARIMA | 30.516% |

Holt-Winters achieved the lowest forecasting error among the evaluated models.

The 2025/26 period was also used during model refinement. Consequently, these results represent retrospective model evaluation rather than performance on a fully independent holdout dataset.


Power BI Dashboard

An interactive four-page Power BI report was developed to communicate NHS emergency care performance, operational pressures and forecasting results.

1. Executive Overview

Provides a high-level summary of NHS emergency care performance, including:

- Total A&E attendances and emergency admissions.
- Four-hour waiting-time breach rate.
- Decision-to-admit waiting-time pressure.
- Historical trends and financial-year filtering.

2. Provider Performance

Examines differences in emergency care performance across NHS providers through:

- Provider-level performance indicators.
- Top-10 provider comparisons.
- Waiting-time performance tables.
- Interactive financial-year filtering.

 3. Emergency Care Pressure

Investigates operational pressures affecting emergency departments, including:

- Four-hour waiting-time breaches.
- Decision-to-admit delays exceeding four hours.
- Monthly pressure trends.
- Annual comparisons of emergency care demand and delays.

4. Demand Forecasting

Presents the results of the time-series forecasting analysis, including:

- Actual versus Holt-Winters predicted A&E attendances.
- Comparison of four forecasting approaches.
- Model accuracy comparisons using MAPE and RMSE.
- A summary of model evaluation findings.

The forecasting dashboard evaluates predictions for April 2025–March 2026 and does not represent a forecast of future demand beyond March 2026.


Repository Structure

The project is organised into four main folders:

Data
Contains seven processed datasets used for the NHS performance analysis, forecasting evaluation and Power BI visualisations.

notebook
Contains the Jupyter notebook used for data collection, cleaning, exploratory analysis and forecasting.

Main file: `01_Data_Collection_and_Cleaning.ipynb`

Power BI
Contains the interactive four-page Power BI report.

Main file: `NHS_Emergency_Care_Intelligence.pbix`

Project Documentation
Contains the PDF project report, including the methodology, analysis, results and conclusions.

Data Source

The project uses publicly available A&E Attendances and Emergency Admissions data published by NHS England.

Official source: https://www.england.nhs.uk/statistics/statistical-work-areas/ae-waiting-times-and-activity/

How to Explore the Project

1. Read the project documentation for the methodology and findings.
2. Open the Jupyter notebook to explore the Python analysis and forecasting workflow.
3. Review the processed datasets in the Data folder.
4. Open the `.pbix` file using Power BI Desktop to explore the interactive dashboards.

Note: The Power BI report may require updating local dataset file paths before refreshing on another computer.