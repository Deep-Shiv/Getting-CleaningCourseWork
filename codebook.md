Merges the training and test sets to create one data set, namely train/X_train.txt with test/X_test.txt, train/subject_train.txt with test/subject_test.txt,  and train/y_train.txt with test/y_test.txt

Reads features.txt and extracts only the measurements on the mean and standard deviation for each measurement. All measurements appear to be floating point numbers in the range (-1, 1).

Reads activity_labels.txt and applies descriptive activity names to name the activities in the data set:

walking

walkingupstairs

walkingdownstairs

sitting

standing

laying

The script also appropriately labels the data set with descriptive names: all feature names (attributes) and activity names are converted to lower case, underscores and brackets () are removed. The result is saved as merged_clean_data.txt.

Finally, the script creates a 2nd, independent tidy data set with the average of each measurement for each activity and each subject. The result is saved as averages_data_set.txt. There are 30 subjects and 6 activities, thus 180 rows in this data set with averages.
