### **Peer-graded Assignment: Getting and Cleaning Data Course Project**

------
This repository is a submission of *Aisa Mijeno* for Getting and Cleaning Data course project. It has the instructions on how to run analysis on Human Activity recognition dataset.
<br>

#### **Project Description**
****
The purpose of this project is to demonstrate your ability to collect, work with, and clean a data set. The goal is to prepare tidy data that can be used for later analysis. You will be graded by your peers on a series of yes/no questions related to the project.
<br>

#### **Dataset**
****
The data linked to from the course website represent data collected from the accelerometers from the Samsung Galaxy S smartphone. A full description is available at the site where the data was obtained:
[Human Activity Recognition Using Smartphones](http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones)

Data for the project:
[Data in zip File](https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip)
<br>

#### **Files in GitHub Repository**
****
`tidy_data.txt` - a tidy data set as described.

`CodeBook.md` - a code book that describes the variables, the data, and any transformations or work that was performed to clean up the data

`README.md` - a readme file that explain about the project.

`run_analysis.R` - performs the data preparation and then followed by the 5 steps required as described in the course project’s definition:


1. Merges the training and the test sets to create one data set.

2. Extracts only the measurements on the mean and standard deviation for each measurement.

3. Uses descriptive activity names to name the activities in the data set

4. Appropriately labels the data set with descriptive variable names.

5. From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.
FinalData.txt is the exported final data after going through all the sequences described above.
<br>

#### **Data Analysis**
****
To perform the data analysis it is required to perform the following **steps**:

* **Clone** this repository into a folder on the local machine: `git clone https://github.com/aisamijeno/Getting-and-Cleaning-Data-Course-Project`

* **Set the Working Directory** to the folder where the Git repository has been cloned:
```
setwd("<Cloned Repo Folder Path>")
```

* **Download and Unzip** the data package above.

* **Source** the run_analysis.R script:
```
source("run_analysis.R")
```
Sourcing the `run_analysis.R` script will perform the actual analysis. In particular:

* Read the Dataset
* Merges the training and the test sets to create one single data set.
* Extracts only the measurements on the mean and standard deviation for each measurement.
* Uses descriptive activity names to name the activities in the data set
* Appropriately labels the data set with descriptive variable names.
* Creates a second, independent tidy data set with the average of each variable for each activity and each subject.

After performing the analysis, the following files will be created:

* `tidy_data.txt` *(corresponding to a `180x68` data frame)*

* Use data: to read and use the data it is necessary to run the following command:

```
data <- read.table("tidy_dataset.txt")
```
