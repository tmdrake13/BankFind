# BankFind
### Overview
This is a collection of Jupyter Python notebooks which 
1. Create a function ```search``` that allows us to interface with the FDIC's BankFind API, and performs searches based on filters and other parameters (see BankFindSearch for more details)
2. Uses the search functionality to perform data analysis using XGBoost

### General Notes
- Most of the data analysis consists of four models in ```MLModels1&2``` and ```MLModels3&4```. Descriptions and more info on these are in the respective worksheets
- ```FinancialPractice``` is an exploratory excercise for me, as the 'financials' endpoint of contains over 1,000 return variables, so I am trying to sift through to see what can be of use
- ```UnitTests``` contains some unit tests for the ```search``` function, as this is the foundation for my data collection
- ```FinalSummaryReport``` is my final summary of findings - it summarizes the problem statements, provides context for the data we are working with, discusses my data analysis, and concludes with my findings.

### Setup
#### To get started, ```git clone``` this repository or download it as a ZIP
Make sure to save the folder somewhere easily accessible (Documents, Desktop, etc)
#### Next, ensure you have Jupyter Notebook installed
Jupyter Notebook is included with the Anaconda Toolkit\
If you don't already have Anaconda installed, download it free from https://www.anaconda.com/products/individual \
Once it's installed, open Jupyter Notebook either from the Anaconda Navigator or directly
#### Once you have Jupyter Notebook opened and running in your web browser,  navigate to ```BankFind```
You can now open the Python notebooks. However, you will likely see errors when trying to run, since the last step is to install some dependencies to python
#### Finally, ```pip install``` some necessary modules
This can be done in the Anaconda Prompt, also included with the Anaconda toolkit\
Run the following:

>```pip install import_ipynb xgboost shap```

- ```xgboost``` is the software used to perform ML analysis on the data
- ```import_ipynb``` helps import the contents of one jupyter notebook to another, aiding in modularizing the code
- ```shap``` is a great tool that helps us visualize and better understand each feature's importance in our model.

