# Detecting Semantic Equivalence of Quora Question Pairs

Lakshya A Agrawal (lakshya18242@iiitd.ac.in) <br>
Shrikant Garg (shrikant18312@iiitd.ac.in) <br>
Bhavya Chopra (bhavya18333@iiitd.ac.in) <br>

Link to dataset: [Kaggle Quora Question Pairs](https://www.kaggle.com/c/quora-question-pairs/data)

### Problem Statement

Popular QnA websites, such as StackExchange, Quora and Yahoo Answers are visited by millions of users on a daily basis, which leads different users to ask separate questions with similar intent. This makes it difficult for users to seek the best answer, and such ‘duplicate’ questions require to be manually moderated to be taken down or merged with similar threads. These repeated questions can result in poor recommendations for the users as well. This motivates us to identify duplicate question pairs on such forums. The learning task is to train a classifier which can predict if a given question pair is semantically equivalent or not with the classes being “equivalent” and “not equivalent”.

### Dataset
The chosen dataset is manually annotated, with a large number of training samples belonging to Quora. The table below shows the training, test and validation set splits. 

| Set            | Samples | Split Ratio |
|----------------|---------|-------------|
| Total Samples  | 404,290 | 1.0         |
| Train Set      | 291,089 | 0.72        |
| Test Set       | 80,858  | 0.2         |
| Validation Set | 42,343  | 0.08        |

The dataset (60 MB) consists of 6 attributes:
 - id: ID for every question pair
 - qid1: Unique ID for first question
 - qid2: Unique ID for second question
 - question1: Text for first question
 - question2: Text for second question
 - is_duplicate: 0 if questions are not duplicates, 1 if questions are duplicates. 

We found the data to be imbalanced (Class_0:Class_1 ratio is 63:37)

<img src="https://github.com/LakshyAAAgrawal/quora-question-pairs/blob/main/assets/plots_data.png" width="600px"></img>

Word cloud for different question pairs:

![alt](https://github.com/LakshyAAAgrawal/quora-question-pairs/blob/main/assets/word_cloud_different.png)

Word cloud for duplicate question pairs:

![alt](https://github.com/LakshyAAAgrawal/quora-question-pairs/blob/main/assets/word_cloud_dups_1.png)

### Slides
![](assets/slides/1.png)
![](assets/slides/2.png)
![](assets/slides/3.png)
![](assets/slides/4.png)
![](assets/slides/5.png)
![](assets/slides/6.png)
![](assets/slides/7.png)
![](assets/slides/8.png)
![](assets/slides/9.png)
![](assets/slides/10.png)
![](assets/slides/11.png)
![](assets/slides/12.png)
![](assets/slides/13.png)
![](assets/slides/14.png)
![](assets/slides/15.png)
![](assets/slides/16.png)
![](assets/slides/17.png)
![](assets/slides/18.png)
![](assets/slides/19.png)
![](assets/slides/20.png)
![](assets/slides/21.png)
![](assets/slides/22.png)
![](assets/slides/23.png)
![](assets/slides/24.png)
![](assets/slides/25.png)
![](assets/slides/26.png)
![](assets/slides/27.png)
![](assets/slides/28.png)
![](assets/slides/29.png)
![](assets/slides/30.png)

### Feature Extraction
<img src="https://github.com/LakshyAAAgrawal/quora-question-pairs/blob/main/assets/plots_EDA.png" width="700px"></img>
<img src="https://github.com/LakshyAAAgrawal/quora-question-pairs/blob/main/assets/feat_ext1.png" width="700px"></img>

### Feature Selection
Pair Plots for all extracted features:

<img src="https://github.com/LakshyAAAgrawal/quora-question-pairs/blob/main/assets/feat_pair_plots.png" width="800px"></img>

### Baseline models

<img src="https://github.com/LakshyAAAgrawal/quora-question-pairs/blob/main/assets/svm-boundary.jpeg"></img>

<img src="https://github.com/LakshyAAAgrawal/quora-question-pairs/blob/main/assets/XGBoost_ROC.png" width="600px"></img>

### Text to Vector approaches

<img src="https://github.com/LakshyAAAgrawal/quora-question-pairs/blob/main/assets/pca.jpeg" width="400px"></img>

<img src="https://github.com/LakshyAAAgrawal/quora-question-pairs/blob/main/assets/feat_plots.png" width="600px"></img>

### Training Neural Networks

### Results and Conclusion
  
