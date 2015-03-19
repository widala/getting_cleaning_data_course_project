run_analyis.R - script for concatenating data sets and making a final tidy data set based on Galaxy S motion data collected from volunteers performing preset activities

The data for this script can be found at:
https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

To run the script, the R working directory should be set to the unzipped file UCI HAR Dataset folder. The final, tidy data set will be created in this file as well.

The goals of the script are to:
  -  Merge the training and test data sets to create one data set
  -  Extract only the measurements on the mean and standard deviation for each measurement 
  -  Uses descriptive activity names to name the activities in the data set
  -  Appropriately labels the data set with descriptive variable names 
  -  Create a second, independent tidy data set with the average of each variable for each activity and subject

The motion data in the data set can be found in the x_train.txt and and x_test.txt files.
The subject ID column was taken from the y_train.txt and y_test.txt files.
The activity column was taken from the y_train.txt and y_test.txt files and interpreted using the activity_labels.txt      file.
The features of the motion data are described in the feature.txt file.
