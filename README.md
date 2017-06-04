# Getting-and-Cleaning-Data-Project
Course project for Getting and Cleaning Data Module for Data Science

The purpose of this project is to demonstrate the ability to collect, work with, and clean a data set. The goal is to prepare tidy data that can be used for later analysis.

The data set used for this project related to waearable computing.

One of the most exciting areas in all of data science right now is wearable computing - see for example this article . Companies like Fitbit, Nike, and Jawbone Up are racing to develop the most advanced algorithms to attract new users. The data linked to from the course website represent data collected from the accelerometers from the Samsung Galaxy S smartphone. 

DataSet Information

The source data set that this project was based on was obtained from the Human Activity Recognition Using Smartphones Data Set, which describes how the data was initially collected as follows:

The experiments have been carried out with a group of 30 volunteers within an age bracket of 19-48 years. Each person performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist. Using its embedded accelerometer and gyroscope, we captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz. The experiments have been video-recorded to label the data manually. The obtained dataset has been randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data.

The sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window). The sensor acceleration signal, which has gravitational and body motion components, was separated using a Butterworth low-pass filter into body acceleration and gravity. The gravitational force is assumed to have only low frequency components, therefore a filter with 0.3 Hz cutoff frequency was used. From each window, a vector of features was obtained by calculating variables from the time and frequency domain.



Repository Files
This repository contains following files:

- README.md , this file, which provides an overview of the data set and how it was created.
- tidy_data.txt , which contains the data set.
- CodeBook.md , the code book, which describes the contents of the data set.
- run_analysis.R , the R script that was used to create the data set (see the Creating the data set section below)


Creating the dataset

1) Download the dataset

2) List all the files of UCI HAR Dataset folder

3) Load activity, subject and feature info. Read data from the files into the variables.

4) Merges the training and the test sets to create one data set.

5) Extracts only the measurements on the mean and standard deviation for each measurement.

6) Uses descriptive activity names to name the activities in the data set.

7) Appropriately labels the data set with descriptive variable names.

8) Creates a independent tidy dataset that consists of the average (mean) value of each variable for each subject and activity pair.

The  tidy_data.txt  in this repository was created by running the  run_analysis.R 