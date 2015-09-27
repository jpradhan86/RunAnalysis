# RunAnalysis
The run_analysis.R file contains the code as follows.

1. Load the activity labels from activity.txt

2. Load the data column names from feature.txt

3. Extract the feature_names that contains the mean and standard deviation.

4. Read the test data from X_test.txt, y_test.txt and subject.txt

5. Take only the features that were extracted in step 3 from X_test.txt to X_test

6. Give name to the Activity_ID in y_test.txt by using the activity labels and store it in y_test

7. column bind the subject, y_test and X_test and form one data set as test_data.

8. Do the same thing for train_data by using steps 4-6

9. Merge both the data as complete_data by using rbind.

10. Melt the complete_data by using Subject, Activity_ID, Activity_Label as id and the rest as measurement variables.

11. Now dcast the above data for generating the mean for each variable and store it in tidy_data.

12. Now write the data in tidy_data to tidy_data.txt

Column Description
------------------
subject: Contains the ID of subject

Activity_ID: ID of the activity

Activity_Label: Contains the corresponding activities for Activity_ID

Rest Columns: mean of the corresponding measurements for each subject and  activity.
