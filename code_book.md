Introduction
The script run_analysis.Rperforms the 5 steps of the course project's task.

Similar data (i.e. files having the same number of columns and referring to the same entities) was merged using the rbind() function.
Columns with the mean and standard deviation measures were taken from the whole dataset using grep(). After extracting these columns, they are given the correct names, taken from features.txt.
We took activity names and IDs from activity_labels.txt and they were substituted in the dataset.
Columns with vague column names were corrected.
We generated a new dataset with average measures for each subject and activity type. The output file is called averages_data.txt.
Variables
train_subjects, train_values, train_activity, test_subjects, test_values, and test_activity contain the data from the downloaded files.
x_data, y_data and subject_data merge the previous datasets.
features contains the correct names for the x_data dataset, which are applied to the column names stored in desired_features.
A similar approach is taken with activity names (i.e. the activity_labels variable).
all_data merges x_data, y_data and subject_data in a unique dataset.
averages_data contains the relevant averages which will be later stored in a .txt file. ddply() from the plyr package is used to apply colMeans().