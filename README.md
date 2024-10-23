# DS4002-Project2

This project explores the hypothesis that higher percentages of medicaid enrollment in each state of the US, along with the adoption of the medicaid expansion policy, will reduce the annual healthcare expenses in the respective states. 

## Software & Platforms
The scripts used to clean and analyze the data were written exclusively in Python, utilizing the seaborn, pandas, and matplotlib libraries to perform time series forcasting with ARIMA and develop graphs to express the results. Furthermore, Google Sheets and Excel were also used to transfer tabular data and create more figures. The platform used was Windows, but the Python notebooks that contain the scripts may run on any operating system that has Python and the respective dependencies downloaded.

## Documentation Map
### Data
This folder consists of the raw and cleaned datasets that were pulled from a source called Centers for Medicare & Medicaid Services. 
- medicaid_enrollment.csv details the annual enrollment in medicaid in each state of the US from the years 2014-2020.
- personal_healthcare_expenses.csv details the annual healthcare costs in each state of the US from the years 2014-2020.
- average_salary_state.csv details the average annual income of each state in the US from the years 2014-2023.
- state_population.csv details the population in each state from the years 2014-2020.
  There is also a Data Appendix file, which follows [this framework](https://www.projecttier.org/tier-protocol/protocol-4-0/root/data/analysisdata/data-appendixfile/) to outline and explain the process behind the variables derived in the [Analysis Data File](tbd).
### Output
This folder contains any materials outputted as a result of data analysis. There were multiple figures created in the notebooks from the SCRIPTS folder:
- *add output*
### Scripts
- exploratory.ipynb: the Python notebook used in exploratory data analysis to briefly describe the data sets and begin cleaning.
- healthcare_analysis.ipynb: the Python notebook that performed the data analysis, starting from cleaning the data, preprocessing it, and running the time series forcasting.
### LICENSE.md
This is the respective license for this project.
## Reproduction Instructions
1. Add data
