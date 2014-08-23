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
    2. run_analysis.R is put in the parent folder of UCI HAR Dataset, then this folder set  as the working directory using setwd() function in RStudio.
    3.source("run_analysis.R") is run to clean up and merge datasets and to generate a new file tidy_data.txt in the working directory.

    Dependency:
    run_analysis.R also installs its dependency libraries automatically. It depends on reshape2 and data.table libraries to run successfully.