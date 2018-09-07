Codebook 

Background
The experiments have been carried out with a group of 30 volunteers within an age bracket of 19-48 years. Each person performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, 
SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist. Using its embedded accelerometer and gyroscope, we captured 3-axial linear acceleration and 3-axial angular 
velocity at a constant rate of 50Hz. The experiments have been video-recorded to label the data manually. The obtained dataset has been randomly partitioned into two sets, where 70% of the volunteers 
was selected for generating the training data and 30% the test data. 
The sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window). 
The sensor acceleration signal, which has gravitational and body motion components, was separated using a Butterworth low-pass filter into body acceleration and gravity. The gravitational force is assumed 
to have only low frequency components, therefore a filter with 0.3 Hz cutoff frequency was used. From each window, a vector of features was obtained by calculating variables from the time and frequency 
domain. See 'features_info.txt' for more details. 

A full description is available at the site where the data was obtained:
	http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

Data source
Here are the data for the project:
	https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip
The original data needs be unzipped and contains the train and test folders, as well as "activity_labels.txt", "features.txt", 'features_info.txt", and "README.txt" files. The train folder contains 4 files: Inertial 
Signals, subject_train.txt, X_train.txt, and y_train.txt. The test folder contains 4 files: Inertial Signals, subject_test.txt, X_test.txt, and y_test.txt.


Steps involved in reading and transforming the data sets:
1. Downloading and unzipping the data set from https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip
2. Reading all files (except the inertial signals files) in the train and test sets. 
3. Reading the "activity_labels.txt", "features.txt"
4. Assigning column names
5. Mergin the data sets
6. Reading column names, and creating a vector for defining the ID, the mean and the standard deviation
7. Making second tidy data set 
8. Writing second tidy data set in txt file

Variables
angle(tBodyAccJerkMean)	fBodyBodyGyroMag-iqr()	tBodyAcc-std()-X
angle(tBodyAccMean	fBodyBodyGyroMag-kurtosis()	tBodyAcc-std()-Y
angle(tBodyGyroJerkMean	fBodyBodyGyroMag-mad()	tBodyAcc-std()-Z
angle(tBodyGyroMean	fBodyBodyGyroMag-max()	tBodyGyro-arCoeff()-X
angle(X	fBodyBodyGyroMag-maxInds	tBodyGyro-arCoeff()-Y
angle(Y	fBodyBodyGyroMag-mean()	tBodyGyro-arCoeff()-Z
angle(Z	fBodyBodyGyroMag-meanFreq()	tBodyGyro-correlation()-X
fBodyAcc-energy()-X	fBodyBodyGyroMag-min()	tBodyGyro-correlation()-Y
fBodyAcc-energy()-Y	fBodyBodyGyroMag-skewness()	tBodyGyro-energy()-X
fBodyAcc-energy()-Z	fBodyBodyGyroMag-sma()	tBodyGyro-energy()-Y
fBodyAcc-entropy()-X	fBodyBodyGyroMag-std()	tBodyGyro-energy()-Z
fBodyAcc-entropy()-Y	fBodyGyro-energy()-X	tBodyGyro-entropy()-X
fBodyAcc-entropy()-Z	fBodyGyro-energy()-Y	tBodyGyro-entropy()-Y
fBodyAcc-iqr()-X	fBodyGyro-energy()-Z	tBodyGyro-entropy()-Z
fBodyAcc-iqr()-Y	fBodyGyro-entropy()-X	tBodyGyro-iqr()-X
fBodyAcc-iqr()-Z	fBodyGyro-entropy()-Y	tBodyGyro-iqr()-Y
fBodyAccJerk-energy()-X	fBodyGyro-entropy()-Z	tBodyGyro-iqr()-Z
fBodyAccJerk-energy()-Y	fBodyGyro-iqr()-X	tBodyGyroJerk-arCoeff()-X
fBodyAccJerk-energy()-Z	fBodyGyro-iqr()-Y	tBodyGyroJerk-arCoeff()-Y
fBodyAccJerk-entropy()-X	fBodyGyro-iqr()-Z	tBodyGyroJerk-arCoeff()-Z
fBodyAccJerk-entropy()-Y	fBodyGyro-kurtosis()-X	tBodyGyroJerk-correlation()-X
fBodyAccJerk-entropy()-Z	fBodyGyro-kurtosis()-Y	tBodyGyroJerk-correlation()-Y
fBodyAccJerk-iqr()-X	fBodyGyro-kurtosis()-Z	tBodyGyroJerk-energy()-X
fBodyAccJerk-iqr()-Y	fBodyGyro-mad()-X	tBodyGyroJerk-energy()-Y
fBodyAccJerk-iqr()-Z	fBodyGyro-mad()-Y	tBodyGyroJerk-energy()-Z
fBodyAccJerk-kurtosis()-X	fBodyGyro-mad()-Z	tBodyGyroJerk-entropy()-X
fBodyAccJerk-kurtosis()-Y	fBodyGyro-max()-X	tBodyGyroJerk-entropy()-Y
fBodyAccJerk-kurtosis()-Z	fBodyGyro-max()-Y	tBodyGyroJerk-entropy()-Z
fBodyAccJerk-mad()-X	fBodyGyro-max()-Z	tBodyGyroJerk-iqr()-X
fBodyAccJerk-mad()-Y	fBodyGyro-maxInds-X	tBodyGyroJerk-iqr()-Y
fBodyAccJerk-mad()-Z	fBodyGyro-maxInds-Y	tBodyGyroJerk-iqr()-Z
fBodyAccJerk-max()-X	fBodyGyro-maxInds-Z	tBodyGyroJerk-mad()-X
fBodyAccJerk-max()-Y	fBodyGyro-mean()-X	tBodyGyroJerk-mad()-Y
fBodyAccJerk-max()-Z	fBodyGyro-mean()-Y	tBodyGyroJerk-mad()-Z
fBodyAccJerk-maxInds-X	fBodyGyro-mean()-Z	tBodyGyroJerkMag-energy()
fBodyAccJerk-maxInds-Y	fBodyGyro-meanFreq()-X	tBodyGyroJerkMag-entropy()
fBodyAccJerk-maxInds-Z	fBodyGyro-meanFreq()-Y	tBodyGyroJerkMag-iqr()
fBodyAccJerk-mean()-X	fBodyGyro-meanFreq()-Z	tBodyGyroJerkMag-mad()
fBodyAccJerk-mean()-Y	fBodyGyro-min()-X	tBodyGyroJerkMag-max()
fBodyAccJerk-mean()-Z	fBodyGyro-min()-Y	tBodyGyroJerkMag-mean()
fBodyAccJerk-meanFreq()-X	fBodyGyro-min()-Z	tBodyGyroJerkMag-min()
fBodyAccJerk-meanFreq()-Y	fBodyGyro-skewness()-X	tBodyGyroJerkMag-sma()
fBodyAccJerk-meanFreq()-Z	fBodyGyro-skewness()-Y	tBodyGyroJerkMag-std()
fBodyAccJerk-min()-X	fBodyGyro-skewness()-Z	tBodyGyroJerk-max()-X
fBodyAccJerk-min()-Y	fBodyGyro-sma()	tBodyGyroJerk-max()-Y
fBodyAccJerk-min()-Z	fBodyGyro-std()-X	tBodyGyroJerk-max()-Z
fBodyAccJerk-skewness()-X	fBodyGyro-std()-Y	tBodyGyroJerk-mean()-X
fBodyAccJerk-skewness()-Y	fBodyGyro-std()-Z	tBodyGyroJerk-mean()-Y
fBodyAccJerk-skewness()-Z	gravity)	tBodyGyroJerk-mean()-Z
fBodyAccJerk-sma()	gravityMean)	tBodyGyroJerk-min()-X
fBodyAccJerk-std()-X	tBodyAcc-arCoeff()-X	tBodyGyroJerk-min()-Y
fBodyAccJerk-std()-Y	tBodyAcc-arCoeff()-Y	tBodyGyroJerk-min()-Z
fBodyAccJerk-std()-Z	tBodyAcc-arCoeff()-Z	tBodyGyroJerk-sma()
fBodyAcc-kurtosis()-X	tBodyAcc-correlation()-X	tBodyGyroJerk-std()-X
fBodyAcc-kurtosis()-Y	tBodyAcc-correlation()-Y	tBodyGyroJerk-std()-Y
fBodyAcc-kurtosis()-Z	tBodyAcc-energy()-X	tBodyGyroJerk-std()-Z
fBodyAcc-mad()-X	tBodyAcc-energy()-Y	tBodyGyro-mad()-X
fBodyAcc-mad()-Y	tBodyAcc-energy()-Z	tBodyGyro-mad()-Y
fBodyAcc-mad()-Z	tBodyAcc-entropy()-X	tBodyGyro-mad()-Z
fBodyAccMag-energy()	tBodyAcc-entropy()-Y	tBodyGyroMag-energy()
fBodyAccMag-entropy()	tBodyAcc-entropy()-Z	tBodyGyroMag-entropy()
fBodyAccMag-iqr()	tBodyAcc-iqr()-X	tBodyGyroMag-iqr()
fBodyAccMag-kurtosis()	tBodyAcc-iqr()-Y	tBodyGyroMag-mad()
fBodyAccMag-mad()	tBodyAcc-iqr()-Z	tBodyGyroMag-max()
fBodyAccMag-max()	tBodyAccJerk-arCoeff()-X	tBodyGyroMag-mean()
fBodyAccMag-maxInds	tBodyAccJerk-arCoeff()-Y	tBodyGyroMag-min()
fBodyAccMag-mean()	tBodyAccJerk-arCoeff()-Z	tBodyGyroMag-sma()
fBodyAccMag-meanFreq()	tBodyAccJerk-correlation()-X	tBodyGyroMag-std()
fBodyAccMag-min()	tBodyAccJerk-correlation()-Y	tBodyGyro-max()-X
fBodyAccMag-skewness()	tBodyAccJerk-energy()-X	tBodyGyro-max()-Y
fBodyAccMag-sma()	tBodyAccJerk-energy()-Y	tBodyGyro-max()-Z
fBodyAccMag-std()	tBodyAccJerk-energy()-Z	tBodyGyro-mean()-X
fBodyAcc-max()-X	tBodyAccJerk-entropy()-X	tBodyGyro-mean()-Y
fBodyAcc-max()-Y	tBodyAccJerk-entropy()-Y	tBodyGyro-mean()-Z
fBodyAcc-max()-Z	tBodyAccJerk-entropy()-Z	tBodyGyro-min()-X
fBodyAcc-maxInds-X	tBodyAccJerk-iqr()-X	tBodyGyro-min()-Y
fBodyAcc-maxInds-Y	tBodyAccJerk-iqr()-Y	tBodyGyro-min()-Z
fBodyAcc-maxInds-Z	tBodyAccJerk-iqr()-Z	tBodyGyro-sma()
fBodyAcc-mean()-X	tBodyAccJerk-mad()-X	tBodyGyro-std()-X
fBodyAcc-mean()-Y	tBodyAccJerk-mad()-Y	tBodyGyro-std()-Y
fBodyAcc-mean()-Z	tBodyAccJerk-mad()-Z	tBodyGyro-std()-Z
fBodyAcc-meanFreq()-X	tBodyAccJerkMag-energy()	tGravityAcc-arCoeff()-X
fBodyAcc-meanFreq()-Y	tBodyAccJerkMag-entropy()	tGravityAcc-arCoeff()-Y
fBodyAcc-meanFreq()-Z	tBodyAccJerkMag-iqr()	tGravityAcc-arCoeff()-Z
fBodyAcc-min()-X	tBodyAccJerkMag-mad()	tGravityAcc-correlation()-X
fBodyAcc-min()-Y	tBodyAccJerkMag-max()	tGravityAcc-correlation()-Y
fBodyAcc-min()-Z	tBodyAccJerkMag-mean()	tGravityAcc-energy()-X
fBodyAcc-skewness()-X	tBodyAccJerkMag-min()	tGravityAcc-energy()-Y
fBodyAcc-skewness()-Y	tBodyAccJerkMag-sma()	tGravityAcc-energy()-Z
fBodyAcc-skewness()-Z	tBodyAccJerkMag-std()	tGravityAcc-entropy()-X
fBodyAcc-sma()	tBodyAccJerk-max()-X	tGravityAcc-entropy()-Y
fBodyAcc-std()-X	tBodyAccJerk-max()-Y	tGravityAcc-entropy()-Z
fBodyAcc-std()-Y	tBodyAccJerk-max()-Z	tGravityAcc-iqr()-X
fBodyAcc-std()-Z	tBodyAccJerk-mean()-X	tGravityAcc-iqr()-Y
fBodyBodyAccJerkMag-energy()	tBodyAccJerk-mean()-Y	tGravityAcc-iqr()-Z
fBodyBodyAccJerkMag-entropy()	tBodyAccJerk-mean()-Z	tGravityAcc-mad()-X
fBodyBodyAccJerkMag-iqr()	tBodyAccJerk-min()-X	tGravityAcc-mad()-Y
fBodyBodyAccJerkMag-kurtosis()	tBodyAccJerk-min()-Y	tGravityAcc-mad()-Z
fBodyBodyAccJerkMag-mad()	tBodyAccJerk-min()-Z	tGravityAccMag-energy()
fBodyBodyAccJerkMag-max()	tBodyAccJerk-sma()	tGravityAccMag-entropy()
fBodyBodyAccJerkMag-maxInds	tBodyAccJerk-std()-X	tGravityAccMag-iqr()
fBodyBodyAccJerkMag-mean()	tBodyAccJerk-std()-Y	tGravityAccMag-mad()
fBodyBodyAccJerkMag-meanFreq()	tBodyAccJerk-std()-Z	tGravityAccMag-max()
fBodyBodyAccJerkMag-min()	tBodyAcc-mad()-X	tGravityAccMag-mean()
fBodyBodyAccJerkMag-skewness()	tBodyAcc-mad()-Y	tGravityAccMag-min()
fBodyBodyAccJerkMag-sma()	tBodyAcc-mad()-Z	tGravityAccMag-sma()
fBodyBodyAccJerkMag-std()	tBodyAccMag-energy()	tGravityAccMag-std()
fBodyBodyGyroJerkMag-energy()	tBodyAccMag-entropy()	tGravityAcc-max()-X
fBodyBodyGyroJerkMag-entropy()	tBodyAccMag-iqr()	tGravityAcc-max()-Y
fBodyBodyGyroJerkMag-iqr()	tBodyAccMag-mad()	tGravityAcc-max()-Z
fBodyBodyGyroJerkMag-kurtosis()	tBodyAccMag-max()	tGravityAcc-mean()-X
fBodyBodyGyroJerkMag-mad()	tBodyAccMag-mean()	tGravityAcc-mean()-Y
fBodyBodyGyroJerkMag-max()	tBodyAccMag-min()	tGravityAcc-mean()-Z
fBodyBodyGyroJerkMag-maxInds	tBodyAccMag-sma()	tGravityAcc-min()-X
fBodyBodyGyroJerkMag-mean()	tBodyAccMag-std()	tGravityAcc-min()-Y
fBodyBodyGyroJerkMag-meanFreq()	tBodyAcc-max()-X	tGravityAcc-min()-Z
fBodyBodyGyroJerkMag-min()	tBodyAcc-max()-Y	tGravityAcc-sma()
fBodyBodyGyroJerkMag-skewness()	tBodyAcc-max()-Z	tGravityAcc-std()-X
fBodyBodyGyroJerkMag-sma()	tBodyAcc-mean()-Y	tGravityAcc-std()-Y
fBodyBodyGyroJerkMag-std()	tBodyAcc-mean()-Z	tGravityAcc-std()-Z
fBodyBodyGyroMag-energy()	tBodyAcc-min()-X	(blank)
fBodyBodyGyroMag-entropy()	tBodyAcc-min()-Y	X.tBodyAcc.mean...X






