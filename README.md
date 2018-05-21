# Getting-and-Cleaning-Data-Week-4-Assignment
This repo was created to complete the week 4 assignment of the "Getting and Cleaning Data" course at Coursera.

First, download and unzip the data file into your R working directory. Second, download the R source code into your R working directory. Finally, execute R source code to generate tidy data file.

## Data Description
The variables in data set X contains of sensor signals measured with waist-mounted smartphone by 30 subjects. In the Y data, the variables indicate activity type that the subjects performed during testing/observation. 

## Code Explanation 
The code combines the training and test data set, and extract partial variables to create another data set with the averages of each variable for each activity.

## New Dataset 
The generated data set contained variables calculated based on the mean and standard deviation. Each row is an average of each acitivy type for all subjects.

## The code was written based on the instruction of this assignment 
-Read training and test dataset into R environment. -Read variable names into R envrionment. -Read subject index into R environment.

1. Merges the training and the test sets to create one data set. Use command rbind to combine training and test set
2. Extracts only the measurements on the mean and standard deviation for each measurement. Use grep command to get column indexes for variable name contains "mean()" or "std()"
3. Uses descriptive activity names to name the activities in the data set Convert activity labels to characters and add a new column as factor
4. Appropriately labels the data set with descriptive variable names. Give the selected descriptive names to variable columns
5. From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject. Use pipeline command to create a new tidy dataset with command group_by and summarize_each in dplyr package
