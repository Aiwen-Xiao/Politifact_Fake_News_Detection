# Politifact Fake News Detection


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

## Model Comparison
![image](https://github.com/Aiwen-Xiao/Politifact_Fake_News_Detection/blob/main/Model%20Performance.png)
 - Overall, the Naive Bayes has the best performance on this classification task. The accuracy of Naive Bayes is 0.67, and the AUC score is 0.74. Both Random Forest and XGBoost perform worse on this dataset.
 - Naive Bayes works well for spam filtering because it is based on the idea that spam messages are more likely to contain certain words or patterns of words than legitimate messages. 
 - Random Forest and XGBoost are better at capturing complex feature interections, while naive bayes is assuming all features being independent. They may be better than Naive Bayes in the tasks when text context are important to capture
