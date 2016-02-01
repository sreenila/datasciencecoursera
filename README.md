# datasciencecoursera
setwd("C:/Users/sreenilad/Coursera/Getting and Cleaning Data/getdata-projectfiles-UCI HAR Dataset/UCI HAR Dataset")


#Read the train dataset and test dataset
subtest<-read.table("./test/subject_test.txt")
xtest<-read.table("./test/x_test.txt")
ytestlabel<-read.table("./test/y_test.txt")
features<-read.table("./features.txt")
subtrain<-read.table("./train/subject_train.txt")
xtrain<-read.table("./train/x_train.txt")
ytrainlabel<-read.table("./train/y_train.txt")

#create a test data frame and train data frame with labels, measurements and subject
testdata<-cbind(subtest,xtest,ytestlabel)
traindata<-cbind(subtrain,xtrain,ytrainlabel)
summary(testdata)
summary(traindata)


#merge testdata and traindata
mergedata<-rbind(testdata,traindata)

#add features to the merged data signifying the variable names
features<-features[,2]
featuresv<-as.vector(features)
newfeatures<-c("Subject",featuresv,"activity")
colnames(mergedata)<-newfeatures

#Extracted the column names with mean and standard deviation measurements.
mergedata1<-mergedata[,grep("mean|std|activity|Subject",colnames(mergedata))]

#Renaming the activity names
actlab<-read.table("activity_labels.txt")
mergedata1$activity[mergedata1$activity==1]<-"Walking"
mergedata1$activity[mergedata1$activity==2]<-"Walking Upstairs"
mergedata1$activity[mergedata1$activity==3]<-"Walking Downstairs"
mergedata1$activity[mergedata1$activity==4]<-"Sitting"
mergedata1$activity[mergedata1$activity==5]<-"Standing"
mergedata1$activity[mergedata1$activity==6]<-"Laying"

#Tidy data set
finaldata<-group_by(mergedata1,Subject,activity)
final<-summarise_each(finaldata,funs(mean))
write.table(final,"tidy.txt",row.name=FALSE)
