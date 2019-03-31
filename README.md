# Getting_and_cleaning_data_assignment
Assignment for getting and cleaning data using R

There are three core variables:

1.Main
2. Test 3. Train
Main : activity_labels Inertial Signals Inertial Signals Test: features subject_test subject_train Train: features.info X_test X_train

README y_test y_train ‘features_info.txt’: Shows information about the variables used on the feature vector. * - ‘features.txt’: List of all features. * - ‘activity_labels.txt’: Links the class labels with their activity name. * - ‘train/X_train.txt’: Training set. * - ‘train/y_train.txt’: Training labels. * - ‘test/X_test.txt’: Test set. *- ‘test/y_test.txt’: Test labels

Analysis shows that you can categorize the data into 4 segments * training set * test set * features * activity labels

Inertial Signal data is not required. Additionally, features and activity label are more for tagging and descriptive than data sets.

Making the Test and Training Set Data
The objective here is to make the test and training data as per the sequence stated above. 4 basic level data sets will be defined and created:

test data set
train data set
features data set
activity labels data set

2. Extracting only the measurements on the mean and standard deviation for each measurement
Here the understanding is to measure the mean and standard deviation values only. This can be possible through different means. Here I am using the grepl function to get the data and create a data set associated with the requirements.

3. Using descriptive activity names to name the activities in the data set

Label the data set with decriptive variable names
Do note that this was already previously done and now I am simply denoting the vecotrs that have the labels

setAllInOne and setForMeanAndStd are the outcomes and solutions

From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject
New tidy set is created in the end.

