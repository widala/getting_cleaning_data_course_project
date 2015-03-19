run_analyis.R - script for concatenating data sets and making a final tidy data set based on Galaxy S motion data collected from volunteers performing preset activities

The data for this script can be found at:
https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

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

The data available in final data set (tidy.txt) are described below:
  -  subject - ID of the volunteer in the motion data study
  -  activity - a descriptive name of the predetermined movements for the volunteers
  -  The following measurements are present in both average [mean()] and average standard deviation [std()] for each       activity and subject (the meaning of each measurement can be found in features_info.txt):
     -  timeBodyAccelerometer...X                  
     -  timeBodyAccelerometer...Y                 
     -  timeBodyAccelerometer...Z              
     -  timeGravityAccelerometer...X           
     -  timeGravityAccelerometer...Y        
     -  timeGravityAccelerometer...Z    
     -  timeBodyAccelerometerJerk...X  
     -  timeBodyAccelerometerJerk...Y
     -  timeBodyAccelerometerJerk...Z
     -  timeBodyGyroscope...X                   
     -  timeBodyGyroscope...Y                      
     -  timeBodyGyroscope...Z                       
     -  timeBodyGyroscopeJerk...X              
     -  timeBodyGyroscopeJerk...Y                 
     -  timeBodyGyroscopeJerk...Z                  
     -  timeBodyAccelerometerMagnitude           
     -  timeGravityAccelerometerMagnitude          
     -  timeBodyAccelerometerJerkMagnitude         
     -  timeBodyGyroscopeMagnitude                 
     -  timeBodyGyroscopeJerkMagnitude
     -  frequencyBodyAccelerometer...X
     -  frequencyBodyAccelerometer...Y
     -  frequencyBodyAccelerometer...Z   
     -  frequencyBodyAccelerometerJerk...X
     -  frequencyBodyAccelerometerJerk...Y
     -  frequencyBodyAccelerometerJerk...Z
     -  frequencyBodyGyroscope...X       
     -  frequencyBodyGyroscope...Y          
     -  frequencyBodyGyroscope...Z                 
     -  frequencyBodyAccelerometerMagnitude    
     -  frequencyBodyBodyAccelerometerJerkMagnitude
     -  frequencyBodyBodyGyroscopeMagnitude     
     -  frequencyBodyBodyGyroscopeJerkMagnitude
