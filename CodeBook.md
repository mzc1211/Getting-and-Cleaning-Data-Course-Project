This is the Code Book for this project. 

How to get to the TidyData.txt:

 1. Download data from the link below and unzip it into working directory of R Studio.
 2. Execute the R script.
 
 ## About the source data: 
 
 The source data are from the Human Activity Recognition Using Smartphones Data Set. A full description is available at the site where the data was obtained: 
 http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones Here are the data for the project: 
 https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip
 
 ## About R script:
 
 File with R code "run_analysis.R" performs the following steps (in accordance assigned task of course work):

  - Download the dataset, unzip the file and read data from the files into the variables.
  
  1. Merges the training and the test sets to create one data set.
  
      1.1. Concatenate the data tables by rows. 
  
      1.2. Set names to variables.
  
      1.3. Merge columns to get the data frame Data for all data.
 2. Extracts only the measurements on the mean and standard deviation for each measurement.
        
      2.1. Subset Name of Features by measurements on the mean and standard deviation
        
      2.2. Subset the data frame Data by seleted names of Features
      
      2.3. Check the structures of the data frame Data

  3. Uses descriptive activity names to name the activities in the data set.
        
        3.1.Read descriptive activity names from “activity_labels.txt"
        
        3.2. Factorize Varibale activity in the data frame Data using descriptive activity names
        
        3.3. check
        
  4. Appropriately labels the data set with descriptive variable names.
   
  5. From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.
  
  ## About variables:
  
  - dataActivityTest, dataActivityTrain, dataSubjectTest, dataSubjectTrain, dataFeaturesTest and dataFeaturesTrain contain the data from the downloaded files. 
  - dataFeaturesNames contains the correct names for the x_data dataset, which are applied to the column names stored in.


