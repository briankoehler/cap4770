# Assignment 6
**Brian Koehler**
**UFID 7551-8931**


## Implementation
This assignment was implemented using a Jupyter Notebook, similar to previous assignments.  The notebook has 4 sections:

* **Package Imports** - Julia packages are added and ScikitLearn imports are made.
* **Data Preprocessing** - Select columns are read from CSV, separated into independent variables and dependent variables, and normalized.
* **Feature Count Evaluation** - The accuracy of a LinearSVC model using PCA feature count ranging from 1-10 is calculated, along with how long it takes to train the PCA model each time.
* **Plotting** - Using the Plots package, the data colleted in the previous section is plotted to demonstrate the relationship between number of PCA features versus accuracy and training time.


## Data
It is expected that the CSV data file is available in the same directory as `a6.ipynb` and named `01_hdp.csv`.  It will be packaged in my submission to be safe.


## Analysis
The plots constructed demonstrate that a greater PCA feature count results in a greater accuracy of a classification model, such as LinearSVC.  The graphed line generally has an upward slope, with an accuracy beginning at below 40% and reaching a maximum at around 46%.

The plots do not indicate much of a relationship between the number of dimensions when training a PCA model, however.  There is the possibility that an even larger number of features could result in greater time, though, but this specific case only had up to 10 features to train on.  Had more floating-point features been included in this study, it is certainly a possibility that a relationship between number of PCA features and training time would have been discovered.


## Packages
This assignment requred the following packages:

* CSV
* DataFrames
* MultivariateStats
* Plots
* PlotThemes
* ScikitLearn