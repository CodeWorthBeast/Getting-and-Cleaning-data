## Johns Hopkins Getting and Cleaning Data Course Project - Data Cleaning Script

This script performs data cleaning steps for a project in the Johns Hopkins "Getting and Cleaning Data" course. 

**Data Source:**

The data comes from the UCI Machine Learning Repository and focuses on human activity recognition using smartphone sensors (details in `codebook.md`).

**Cleaning Steps:**

1. **Merge Training and Testing Sets:** Combines the training and testing data into a single dataset for analysis.
2. **Feature Selection:** Extracts only the mean and standard deviation measurements for each feature, focusing on summary statistics.
3. **Descriptive Activity Names:** Replaces activity labels with more descriptive names based on the provided mapping.
4. **Variable Naming:** Assigns clear and informative names to the remaining variables based on their origin.
5. **Tidy Data Creation:** Reshapes the data into a "tidy" format using `reshape2` package. This format allows for easier analysis with functions like `dcast` for calculating means by subject and activity.
6. **Mean Calculation:** Calculates the average value for each variable across each activity and subject.

**Output:**

The cleaned data is saved as a new file named "tidyData.txt" in a comma-separated format (CSV). This data is ready for further analysis tasks.

**Dependencies:**

This script requires the following R packages:

* `data.table`: for efficient data manipulation
* `reshape2`: for data reshaping and aggregation

**Instructions:**

1. Ensure you have R and the required packages installed.
2. Download the data from the provided URL (`https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip`). 
3. Run the script to perform the cleaning steps and generate the "tidyData.txt" file.

**Additional Information:**

* Refer to `codebook.md` for a detailed description of the data and its attributes.
* This script provides a basic cleaning workflow. Further cleaning or feature engineering might be needed depending on your specific analysis goals.
