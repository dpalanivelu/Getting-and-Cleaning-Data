# Introduction

The script `run_analysis.R`performs the 5 steps described in the course project's instruction

* Rbind() function is used to merge similar data.
* Only those columns with the mean and standard deviation measures are taken from the whole dataset. After extracting these columns, the correct column names are assigned, taken from `features.txt`.
* Dscriptive activity names are and IDs are applied to the data set by reading the values from from `activity_labels.txt`.
* The data set is appropriately labeled with descriptive variable names.
* Finally the code generates a new dataset with all the average measures for each subject and activity type. The output file is called `averagesdata.txt` and uploaded to the repository.

# Variables

* `xtrain`, `ytrain`, `xtest`, `ytest`, `subjecttrain` and `subjecttest` contain the data from the downloaded files.
* `xdata`, `ydata` and `subjectdata` merge the previous datasets.
* `featuresset` contains the correct names for the `xdata` dataset, which is applied to the column names stored in `mean_and_std_features_set`, a numeric vector used to extract the desired data.
* `alldata` merges `xdata`, `ydata` and `subjectdata` in a dataset.
* 'averages_data` contains the relevant averages which will be later stored in a `.txt` file.