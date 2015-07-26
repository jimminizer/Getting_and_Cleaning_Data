#Code Book
Original data source: https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

Full description of the data source: http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones 

The R Script named "run_analysis.R" performs the data cleansing as following:
* Merges the training and the test sets to create one data set.
                 

                Merge train/X_train.txt with test/X_test.txt, that will come out with a 10299x561 data frame
                Merge train/subject_train.txt with test/subject_test.txt, that will produce a result of 10299x1
                Merge train/y_train.txt with test/y_test.txt, it will also generate a result of 1099x1 with the activity IDs.
* Loading features.txt and extract only the measurements on the mean and standard deviation for each measurement. 
* Uses descriptive activity names to name the activities in the data set:

        walkingupstairs
        
        walking
        
        walkingdownstairs
        
        sitting
        
        standing
        
        laying
* Appropriately labels the data set with descriptive variable names. 
        

        tbodyacc-mean-x 
        
        tbodyacc-mean-y 
        
        tbodyacc-mean-z 
        
        tbodyacc-std-x 
        
        tbodyacc-std-y 
        
        tbodyacc-std-z 
        
        tgravityacc-mean-x 
        
        tgravityacc-mean-y

* From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.
