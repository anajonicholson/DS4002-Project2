# DS4002-Project2
This project explores the hypothesis that higher percentages of Medicaid enrollment in each state of the United States, along with the adoption of the Medicaid expansion policy, will reduce the annual personal healthcare expenses in each respective state. 

## Software & Platforms
The scripts used to clean and analyze the data were written exclusively in Python, utilizing the seaborn, pandas, and matplotlib libraries to perform time-series fitting and forecasting with the ARIMA model and develop graphs to express the results. Furthermore, Google Sheets and Excel were also used to transfer tabular data and create more figures. The platform used was Windows, but the Python notebooks that contain the scripts may run on any operating system that has Python and the respective dependencies downloaded.

## Documentation Map
### DATA
This folder consists of the raw and cleaned datasets that were pulled from the Centers for Medicare & Medicaid Services, United States Census, and Federal Reserve for Economic Data. These are all the original data files that were downloaded from the respective sources. 
* [medicaid_enrollment.csv](https://github.com/anajonicholson/DS4002-Project2/blob/main/DATA/medicaid_enrollment.csv) details the annual enrollment in Medicaid in each state of the US from the years 2014-2020.
* [personal_healthcare_expenses.csv](https://github.com/anajonicholson/DS4002-Project2/blob/main/DATA/personal_healthcare_expenses.csv) details the net annual healthcare costs in each state of the US from the years 2014-2020.
* [average_salary_state.csv](https://github.com/anajonicholson/DS4002-Project2/blob/main/DATA/average_salary_state.csv) details the average annual income of each state in the US from the years 2014-2023.
* [state_population.csv](https://github.com/anajonicholson/DS4002-Project2/blob/main/DATA/state_population.csv) details the population in each state from the years 2014-2020.
* [results.csv](https://github.com/anajonicholson/DS4002-Project2/blob/main/DATA/results.csv) details the results from the ARIMA model analysis, with its collected coefficients and statistics. 

Each of these data files, with the exception of the salary dataset, comes with its own cleaned version, which has been entirely preprocessed and used in the following scripts for this project's analysis. 

There is also a Data Appendix file, which follows [this framework](https://www.projecttier.org/tier-protocol/protocol-4-0/root/data/analysisdata/data-appendixfile/) to outline and explain the process behind the variables derived in the [Analysis Data File](https://github.com/anajonicholson/DS4002-Project2/blob/main/SCRIPTS/healthcare_analysis.ipynb).

### OUTPUT
This folder contains any materials outputted as a result of data analysis. There were multiple figures created in the notebooks from the SCRIPTS folder:
* Effect_of_Medicaid_By_State.png
* Effect_of_Medicaid_Significant_States.png
* Effect_of_Medicaid_States_Without_Expansion_Policy.png
* Moving_Average_Data_By_State.png

### SCRIPTS
- exploratory.ipynb: the Python notebook used in exploratory data analysis to briefly describe the data sets and begin cleaning.
- healthcare_analysis.ipynb: the Python notebook that performed the data analysis, starting from cleaning the data, preprocessing it, and running the time series forecasting.

### LICENSE.md
This is the respective license for this project.

## Reproduction Instructions
1. Open the analysis.ipynb Python notebook from the SCRIPTS folder. This file has all of the necessary information to clean, process, and perform sentiment analysis on the original data sets. For this project, the .ipynb file may be opened in [Google Colab](https://colab.research.google.com/) using a GitHub link (File > Open Notebook > GitHub > [analysis.ipynb](https://github.com/anajonicholson/DS4002-Project2/blob/main/SCRIPTS/healthcare_analysis.ipynb)) or manually downloading and uploading the file into Google Colab. 

Alternatively, this can be run locally in any IDE (Visual Studio Code, IntelliJ, etc.). This operates under the assumption that the user already has a version of [Python](https://www.python.org/downloads/) downloaded onto their operating system.

1. Download the analysis.ipynb from the SCRIPTS folder.
2. Open analysis.ipynb in the IDE of choice. 
3. Run the notebook. In VS Code, there is a "Run All" button that appears in the top row of the tab where the notebook opens. The first 'pip' command listed in the notebook should download all dependencies automatically (with permission given to the kernel if there is a pop-up window), but if not, open a new terminal by clicking the three dots in the top window > Terminal > New Terminal, and type in the recommended 'pip' installation commands as suggested by the IDE. Any other modules that are not on a given user's local machine may be installed with the command "pip install {module_name}", which may happen with the statsmodels module.

Both of these methods will produce all of the figures as seen in the OUTPUT folder as well as the model results in results.csv from the DATA folder. 
