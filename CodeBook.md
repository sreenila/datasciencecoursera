# Code Book

## Activity
Activities consist of the following:
Laying, Sitting, Standing, Walking, Walking Downstairs, Waking Upstairs

tBodyAcc-mean()-X
tBodyAcc-mean()-Y
tBodyAcc-mean()-Z
tBodyAcc-std()-X (dbl) 
tBodyAcc-std()-Y (dbl)
tBodyAcc-std()-Z (dbl),
tGravityAcc-mean()-X (dbl)
tGravityAcc-mean()-Y (dbl)
tGravityAcc-mean()-Z (dbl)
tGravityAcc-std()-X (dbl)
tGravityAcc-std()-Y (dbl)
tGravityAcc-std()-Z (dbl)
tBodyAccJerk-mean()-X (dbl)
tBodyAccJerk-mean()-Y (dbl)
tBodyAccJerk-mean()-Z (dbl)
tBodyAccJerk-std()-X (dbl)
tBodyAccJerk-std()-Y (dbl)
tBodyAccJerk-std()-Z (dbl)
tBodyGyro-mean()-X (dbl)
tBodyGyro-mean()-Y (dbl)
tBodyGyro-mean()-Z (dbl)
tBodyGyro-std()-X(dbl)
tBodyGyro-std()-Y (dbl)
tBodyGyro-std()-Z (dbl)
tBodyGyroJerk-mean()-X(dbl)
tBodyGyroJerk-mean()-Y (dbl)
tBodyGyroJerk-mean()-Z (dbl)
tBodyGyroJerk-std()-X (dbl)
tBodyGyroJerk-std()-Y (dbl)
tBodyGyroJerk-std()-Z (dbl)
tBodyAccMag-mean() (dbl)
tBodyAccMag-std() (dbl)
tGravityAccMag-mean() (dbl)
tGravityAccMag-std() (dbl)
tBodyAccJerkMag-mean() (dbl)
tBodyAccJerkMag-std() (dbl)
tBodyGyroMag-mean() (dbl),
tBodyGyroMag-std() (dbl)
tBodyGyroJerkMag-mean() (dbl)
tBodyGyroJerkMag-std() (dbl)
fBodyAcc-mean()-X (dbl)
fBodyAcc-mean()-Y (dbl)
fBodyAcc-mean()-Z (dbl)
fBodyAcc-std()-X(dbl)
fBodyAcc-std()-Y (dbl)
fBodyAcc-std()-Z (dbl)
fBodyAcc-meanFreq()-X (dbl)
fBodyAcc-meanFreq()-Y (dbl)
fBodyAcc-meanFreq()-Z (dbl)
fBodyAccJerk-mean()-X (dbl)
fBodyAccJerk-mean()-Y (dbl)
fBodyAccJerk-mean()-Z (dbl)
fBodyAccJerk-std()-X (dbl)
fBodyAccJerk-std()-Y (dbl)
fBodyAccJerk-std()-Z (dbl)
fBodyAccJerk-meanFreq()-X (dbl)
fBodyAccJerk-meanFreq()-Y (dbl)
fBodyAccJerk-meanFreq()-Z (dbl)
fBodyGyro-mean()-X (dbl)
fBodyGyro-mean()-Y (dbl)
fBodyGyro-mean()-Z (dbl)
fBodyGyro-std()-X (dbl)
fBodyGyro-std()-Y(dbl)
fBodyGyro-std()-Z (dbl)
fBodyGyro-meanFreq()-X (dbl)
fBodyGyro-meanFreq()-Y (dbl)
fBodyGyro-meanFreq()-Z (dbl)
fBodyAccMag-mean() (dbl)
fBodyAccMag-std() (dbl)
fBodyAccMag-meanFreq() (dbl)
fBodyBodyAccJerkMag-mean() (dbl)
fBodyBodyAccJerkMag-std()(dbl)
fBodyBodyAccJerkMag-meanFreq()(dbl)
fBodyBodyGyroMag-mean() (dbl)
fBodyBodyGyroMag-std() (dbl)
fBodyBodyGyroMag-meanFreq() (dbl)
fBodyBodyGyroJerkMag-mean()(dbl)
fBodyBodyGyroJerkMag-std() (dbl)
fBodyBodyGyroJerkMag-meanFreq() (dbl)

Description of the variables:
The features selected for this database come from the accelerometer and gyroscope 3-axial raw signals tAcc-XYZ and tGyro-XYZ. These time domain signals (prefix 't' to denote time) were captured at a constant rate of 50 Hz. Then they were filtered using a median filter and a 3rd order low pass Butterworth filter with a corner frequency of 20 Hz to remove noise. Similarly, the acceleration signal was then separated into body and gravity acceleration signals (tBodyAcc-XYZ and tGravityAcc-XYZ) using another low pass Butterworth filter with a corner frequency of 0.3 Hz. 

Subsequently, the body linear acceleration and angular velocity were derived in time to obtain Jerk signals (tBodyAccJerk-XYZ and tBodyGyroJerk-XYZ). Also the magnitude of these three-dimensional signals were calculated using the Euclidean norm (tBodyAccMag, tGravityAccMag, tBodyAccJerkMag, tBodyGyroMag, tBodyGyroJerkMag). 

Finally a Fast Fourier Transform (FFT) was applied to some of these signals producing fBodyAcc-XYZ, fBodyAccJerk-XYZ, fBodyGyro-XYZ, fBodyAccJerkMag, fBodyGyroMag, fBodyGyroJerkMag. (Note the 'f' to indicate frequency domain signals). 

These signals were used to estimate variables of the feature vector for each pattern:  
'-XYZ' is used to denote 3-axial signals in the X, Y and Z directions.

tBodyAcc-XYZ
tGravityAcc-XYZ
tBodyAccJerk-XYZ
tBodyGyro-XYZ
tBodyGyroJerk-XYZ
tBodyAccMag
tGravityAccMag
tBodyAccJerkMag
tBodyGyroMag
tBodyGyroJerkMag
fBodyAcc-XYZ
fBodyAccJerk-XYZ
fBodyGyro-XYZ
fBodyAccMag
fBodyAccJerkMag
fBodyGyroMag
fBodyGyroJerkMag

The set of variables that were estimated from these signals are: 

mean(): Mean value
std(): Standard deviation
mad(): Median absolute deviation 
max(): Largest value in array
min(): Smallest value in array
sma(): Signal magnitude area
energy(): Energy measure. Sum of the squares divided by the number of values. 
iqr(): Interquartile range 
entropy(): Signal entropy
arCoeff(): Autorregresion coefficients with Burg order equal to 4
correlation(): correlation coefficient between two signals
maxInds(): index of the frequency component with largest magnitude
meanFreq(): Weighted average of the frequency components to obtain a mean frequency
skewness(): skewness of the frequency domain signal 
kurtosis(): kurtosis of the frequency domain signal 
bandsEnergy(): Energy of a frequency interval within the 64 bins of the FFT of each window.
angle(): Angle between to vectors.
