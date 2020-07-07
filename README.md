Corona Virus has literally given us the ultimate long pause in our life. It has affected so many people from so many countries and still the wave doesn't seem to stop.

 In my project "Corona - Lockdown1.0", I have scraped the tweets from the Lockdown period(India) and tried to analyse and predict the sentiments of the people.
The tweets were scraped by using the "Twint" library with various search keywords like "Lockdown", "Corona", "Work from Home", "PPE". I coded a seperate script for the Tweets Extraction process. The tweets fetched were from the time period of 24 March 2020 - 17 April 2020. I began by analyzing the training set as well as the Lockdown1.0 dataset. Visualisation techniques like word cloud, bar graphs was used to find the trends.

Then comes the most interesting as well as the most cumbersome part - the text processing part! It began with cleaning the tweets by removing emojis, http and other punctuation marks. Stops words have been removed too! Then the tweets were tokenized. TfIdf Transformer was used to normalize the tweets. These steps are really necessary in the text  processing. 

After the completion of the EDA, Visualisation came another important phase,  applying the model on the training set. The training set was a general Sentiment Analysis Training set which was pre labelled into positive or negative sentiment. "Naive Bayes" model was been used and gave an accuracy of arround 77% on the test set. Confusion matrix showed pretty decent results too! The model was then used to predict the sentiments on the Lockdown1.0 dataset. I have also given some user input text to check if the model predicts well.

Conclusion -
-The model predicted that 89.64% of the people were unhappy with the Lockdown1.0 or tweeted something which was negative.
-10.36% people tweeted positive or were happy with the Lockdown.
-The model can be improved by using Watson Tone Analyser, Natural Language Understanding or any other tools to predict the sentiments more accurately.
-Since many of the tweets by Indians contain Hinglish words, text processing becomes a cumbersome task.

Future Scope - 
- Improving the model or choosing a different model.
- Analyzing and predicting the sentiments of the people during Lockdown 2,3,4.
