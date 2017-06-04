# Getting-and-Cleaning-Data-Project
Course project for Getting and Cleaning Data Module for Data Science

The experiments were carried out with a group of 30 volunteers within an age bracket of 19-48 years. They performed a protocol of activities composed of six basic activities: three static postures (standing, sitting, lying) and three dynamic activities (walking, walking downstairs and walking upstairs). The experiment also included postural transitions that occurred between the static postures. These are: stand-to-sit, sit-to-stand, sit-to-lie, lie-to-sit, stand-to-lie, and lie-to-stand. All the participants were wearing a smartphone (Samsung Galaxy S II) on the waist during the experiment execution. We captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz using the embedded accelerometer and gyroscope of the device. The experiments were video-recorded to label the data manually. The obtained dataset was randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data. 



The data set that this code book pertains to is located in the  tidy_data.txt  file of this repository.

Data

The  tidy_data.txt  data file is a text file, containing space-separated values.
The first row contains the names of the variables, which are listed and described in the Variables section, and the following rows contain the values of these variables.



Variables

Identifiers

subject -   ID of the 30 volunteers who performed the activity. Range is from 1 to 30
activity -  Activity type that the 30 volunteers who performed the activity as listed below:
- WALKING : subject was walking
- WALKING_UPSTAIRS : subject was walking upstairs
- WALKING_DOWNSTAIRS : subject was walking downstairs
- SITTING : subject was sitting
- STANDING : subject was standing
- LAYING : subject was laying



Transformations

The zip file containing the source data is located at https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip.

The following transformations were applied to the source data:


1.Read data from the files into the variables.
?Read the Activity files.
?Read the Subject files.
?Read Features files.


2.Merges the training and the test sets to create one data set.
?Concatenate the data tables by rows.
?set names to variables.
?Merge columns to get the data frame Data for all data.


3.Extracts only the measurements on the mean and standard deviation for each measurement.
?Subset Name of Features by measurements on the mean and standard deviation.
?Subset the data frame Data by selected names of Features.


4.Uses descriptive activity names to name the activities in the data set.
?Read descriptive activity names from  activity_labels.txt 
?Factorize variable activity in the data frame Data using descriptive activity names.


5.Appropriately labels the data set with descriptive variable names.


6.Creates a independent tidy dataset that consists of the average (mean) value of each variable for each subject and activity pair.

Final output file is  tidydata.txt 


