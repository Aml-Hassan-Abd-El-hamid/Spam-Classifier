# Spam Classifier
This notebook is built to classify messages into 2 categories: spam or ham based on their text content<br>
The dataset contains 4825 ham messages and 747 and those are their word clouds before cleaning: <br>
<img src="https://github.com/Aml-Hassan-Abd-El-hamid/Spam-Classifier/blob/main/download.png" width="270" height="170" ><br>As you can see in the Ham word cloud some of the most famous words are [ will, u ] which aren't so helpful as they give us no good information regarding the meaning of the messages, and also you can see that words like "text" and "txt" are treated like 2 different words although they have the same meaning, So I followed the next steps to clean the data:<br>
- Lowered case all the words
- Retained alphabetic words only.
- Removed all stop words.
- Replaced "txt" with "text" ** still searching for a better solution for such a problem **.
- Implemented Lemmatization.

Now looking at the ham word cloud again, we can see better results:<br>
<img src="https://github.com/Aml-Hassan-Abd-El-hamid/Spam-Classifier/blob/main/download%20(1).png" width="270" height="170" ><br>
For vectorization, I used the counterVectorizer, I also tried to use TF-IDF vectorization but didn't get good results!<br>
I tried different models and the best one was: **Naive Bayes**, its F1 score is 94% and you can see the confusion matrix below:<br>
<img src="https://github.com/Aml-Hassan-Abd-El-hamid/Spam-Classifier/blob/main/download%20(2).png" width="270" height="270" ><br>



