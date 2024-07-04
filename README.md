# Sentiment-Analysis-with-Naive-Bayes
<h2>Steps involved</h2>
<div>
<h3>Preprocessing Step</h3>
<ul>
<li>Preprocessing of text by removing links, hashtags and any unneeded characters
<li>Stemming of words using Porter Stemmer
<li>Converting all text to lowercase
<li>Removing of all stop words
<li>Tokenize words
</ul>
</div>
<div>
<h3>Model Building steps</h3>
<ul>

<li>build_freq_dict which takes all the tweets and their labels, this produces the frequency dictionary which is the frequency of each word in the positive tweets and negative tweets
<li>get_total_pos_neg_frequency function calculates the total number of wordsin the positive tweets and total number of words in negative tweets
<li>build_probability function calculates the probability of each word given if it is classified as negative or positive P(Word|pos) and P(word|neg), which is calculated using the given formula
<div><img src="https://miro.medium.com/v2/resize:fit:1011/1*7fCiWdownuuotu0T-9nsOg.png"></div>
<li>build_naive_inference function which computes the prediction for each tweet by using the laplacian smoothing to calculate log liklihood and adding the log prior to it using the given formula
<div>
<img src="https://miro.medium.com/v2/resize:fit:1400/1*TYKrmbwVU5rYOszmxqUdXg.png">
</div>

</ul>
</div>

<div>
<h3>Performance Metric</h3>
<ul>
<li>Accuracy is calculated
</ul>
</div>
<div>
<h3>Model Testing</h3>
<ul>
<li>naive_predict function is the predict function which takes the input sentence to be classified as positive or negative and produces the prediciton as class 0 or 1 
</ul>
</div>


