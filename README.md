Course-Project-for-Getting-and-Cleaning-Data-
=============================================
This Project created an R script called run_analysis.R that does the following.

    1.Merges a training and a test set to create one data set.
    2.Extracts only the measurements on the mean and standard deviation for each measurement.
    3.Provides descriptive activity names to name the activities in the merged data set
    4.Appropriately labels the data set with the descriptive activity names.
    5.Creates a second, independent tidy data set with the average of each variable for each activity and each subject.

Steps used to work on project:
  
    1.Downloaded the data source into a folder on the local drive. Creating UCI HAR Dataset folder.
    2. run_analysis.R is put in the parent folder of UCI HAR Dataset, then this folder  is set as the working directory using setwd() function in RStudio.
    3.the command source("run_analysis.R") is run to clean up and merge datasets and to generate a new file tidy_data.txt in the working directory.

Dependency:
    run_analysis.R also installs its dependency libraries automatically. It depends on reshape2 and data.table Packages to run successfully.
    
The run_analysis.R script will perform the following steps:

 Require reshape2 library (for the melt() function)
 Ensure the data path exists (./data)
 Checks if the data set archive was already downloaded
 Downloading the data set archive if it was not already
 Extracts the data set files from the archive
 Reads training & test column files into respective x,y,s variables
 Reads feature names and sets column/variable names respectively
 Creates a unified data set (data frame)
Extracts measurements on mean & standard deviation, for each measurement
Sets activity names on the class labels
Labels data with descriptive variable/column names by removing special characters in the column names and by replacing hyphen's with underscores in the column names
Melts the data set (hence the need for reshape2 library)
Creates an independent, tidy data set which contains the average of each variable for each activity and subject
Saves the resulting tidy data set to file