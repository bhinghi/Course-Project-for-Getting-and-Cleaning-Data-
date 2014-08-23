CodeBook:

   This codebook describes the variables,data, and all transformations  performed to clean up  and obtain the tidy dataset.

Data source:

  Original dataset obtained from:https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip 
 
 Description of the dataset can be found at: http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

Data Set Information

   The experiments were done with a group of 30 volunteers within an age bracket of 19-48 years. Each person performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist. 
   Using its embedded accelerometer and gyroscope, we captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz. The experiments have were video-recorded to label the data manually. 
   The obtained dataset was randomly partitioned into two sets,  70% of which formed the training data and 30% the test dataset.

   Sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled in fixed-width sliding windows 
 
The Data

  The dataset includes the following files:
  
  README.txt

  'features_info.txt': Shows information about the variables used on the feature vector.

  'features.txt': List of all features.

  'activity_labels.txt': Links the class labels with their activity name.

  'train/X_train.txt': Training set.

 'train/y_train.txt': Training labels.

 'test/X_test.txt': Test set.

 'test/y_test.txt': Test labels.


 Transformation Details

  1. Training and  Test datasets merged to create one data set.
  2. Measurements on the mean and standard deviation for each measurement Extracted.
  3. Descriptive activity names used to name the activities in the data set
  4. Data set labels appropriately labelled with descriptive activity names.
  5. Independent tidy dataset with the average of each variable for each activity and each subject created.

The R script`run_analysis.R` is used to achieve the transformation detailed above:

The R script 'run_analysis. R' require ``reshapre2``` and ```data.table``` libraries in R packages to function.
