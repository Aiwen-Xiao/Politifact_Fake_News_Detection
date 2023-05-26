# Politifact_Fake_News_Detection


### Background
The dataset contains 21,152 statements that are fact checked by experts collected from a popular fact check website PolitiFact. There are also sources of statement contained in dataset. Facing such a large amount of misinformation on social media, it is challenging to distinguish the fake news. It would be interesting to try to find linguistic patterns in false political statement. Also, there may be patterns lying under sources , statement date and statement originators of those fake news.
![pic.jpeg](attachment:pic.jpeg)

- Task (Binary text classification): Train a classifier for distinguishing fake political statements. 

- Data Source: https://www.kaggle.com/datasets/rmisra/politifact-fact-check-dataset

- Models: Naive Bayes classifier, Random forest and XGBoost

### Data Description
 - Data Source: https://www.kaggle.com/datasets/rmisra/politifact-fact-check-dataset
 - Data Description:
   - verdict (categorical): The verdict of fact check in one of 6 categories {true, mostly-true, half-true, mostly-false, false, and pants-fire}
   - statement (text): statement being fact checked
   - statement_source (categorical): the source where the statement was made. It is one of 13 categories: {speech,television,news,blog,social_media,advertisement,campaign,meeting,radio,email,testimony,statement,other}

