**Target Variable:** Did the patient seek treatment?
**Overall Question:** What factors determine when Female Mental Health patients seek treatment?

**Data Selection:** 
Our initial process of selecting data started on Kaggle. We were looking for a dataset that had over 1,000 rows, and that had lots of categorical data for us to analyze. This is how we ended up finding the ‘Mental_Health_Dataset’ we are using as it contained the specified constraints we needed. As a team we were able to figure out that each row represents a person, and contains information on their current mental state. This dataset offered lots of categorical data for us to use such as family history, days indoors, mood swings, etc., that we would be comparing to treatment status in order to see if certain factors have an influence. 

**Data Cleaning:**
Our data cleaning was all done in Python where we started with removing columns keeping only gender, family history, treatment, days indoors, growing stress, changes in habits, and mood swing columns in the dataset. After deleting rows we realized we were working with a large dataset so we decided to focus on analyzing just Female patients and to drop all columns with Male patients. We then split our dataset which consisted of only Females into 3 different datasets which consisted of a Testing Dataset (70%) and the Training/ Validation Dataset (30%). Next, we created a dummy variable for most of our categorical data which was gender, family history, treatment, growing stress, changes in habit, and mood swings turning them into binary data with 0 representing yes and 1 representing no. Our days indoors also had to be converted to binary but it had more than 2 categories so we converted it as 0= going out every day,  1=1-14 days, 2 =15-30 days, 3 =31-60 days, and 4 =2 or more months. These conversions allowed us to more easily put our data into our models. 

**Data Visualization:**
Once the data of the dataset was cleaned our team analyzed the data to see which model would best accurately predict if female mental health patients sought treatment. In the Training Phase, our team inputted the first 70% of the data set into a Decision Tree. In making this model it was challenging for the code to clearly represent the statistics present since the font size and distance of the model were compacted. To fix this we utilized the “dpi” attribute to clearly view the data. From this decision tree, the initial conclusion was that the number of days indoors was an important indicator for those looking into treatment, and those experiencing mood swings were more sensitive to not choosing treatment. After training the data, th next 30% of the data was used in the Testing Phase represented by a Confusion matrix. The interpretation of the data from this matrix was about 68.78% accuracy in predicting which patient would seek treatment. With this being above average it clarifies that on average our data is more likely to be accurate when predicting whether women will seek treatment based on these symptoms.








