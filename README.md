# Cousera Getting and Cleaning Data Course Project
One of the most exciting areas in all of data science right now is wearable computing. Companies like Fitbit, Nike, and Jawbone Up are racing to develop the most advanced algorithms to attract new users. The data linked to from the course website represent data collected from the accelerometers from the Samsung Galaxy S smartphone. A full description is available at the site where the data was obtained:

http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

Here are the data for the project:

https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

** Important note: ** in the R script `run_analysis.R` line 11 sets the working directory to the location where the data set for my project was unzipped. This line must be edited for each user to set to the working directory to the location where the user unzipped the UCI HAR Dataset.

The R script called `run_analysis.R` does the following:

1. Sets the working directory to location where UCI HAR Dataset was unzipped
2. Loads the activity and feature info and labels the data set with descriptive variable names
3. Loads both the training and test datasets, keeping only those columns which reflect a mean or standard deviation
4. Loads the activity and subject data for each dataset, and merges those columns with the datasets
5. Merges the training and the test sets to create one data set
6. Converts the `activity` and `subject` columns into factors
7. Creates a tidy dataset that consists of the average (mean) value of each variable for each subject and activity pair

The resulting tidy data is shown in the file `tidy.txt`.
