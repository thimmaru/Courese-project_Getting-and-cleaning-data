		1. Download the source data from the link below and unzip it to working directory of R Studio.
		2. Write and Run an R script.
		Source data:
    The source data used for the project is the Human Activity Recognition Using Smartphones Data Set. 
    A full description is available at the site from where the data was obtained from :http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones Here are the data for the project: https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip
		
		R Script:
		"run_analysis.R" file with the code to perform the following 5 steps (As per assignedcourse work):
			Step 0. Create directory, downloading the dataset from the source and unzip
      url for the dataset source for the project:
      Unzip dataSet to the directory-Data
      R script 'run_analysis.R' to do the following
      Step 1.to merge the training and the test sets to create one data set
         1.1 Read the files
            #1.1.1 Read training tables:
            # 1.1.2 Read test dataset tables:
            # 1.1.3 Read the feature vector:
            # 1.1.4 Read activity labels:
          1.2 Assign column names:
          1.3 Merge all the data in to one set:
      Step 2.Extract only the measurements on the mean and standard deviation for each measurement.
            2.1 Read column names:
            2.2 Create vector for defining ID, mean and standard deviation:
            2.3 Make nessesary subset from setAllInOne:
      Step 4. Label the data set with appropriate descriptive variable names.
      Step 5. From the data set in step 4, create a second, independent tidy data set with average of each variable for each activity and each subject.
            5.1 Make a second tidy data set
		PS. The code assumes that all the data is present in the same folder, un-compressed and without names altered.
		
    variables:
			§ x_train, y_train, x_test, y_test, subject_train and subject_test contain the data from the downloaded files.
			§ x_data, y_data and subject_data merge the previous datasets to further analysis.
			§ features contains the correct names for the x_data dataset, which are applied to the column names.
