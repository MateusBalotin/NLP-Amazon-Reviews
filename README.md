# NLP-Amazon-Reviews

<h1> Objective </h1>
<p>

The goal of this project was to do a sentiment analisys on Amazon Reviews dataset and try to predict the sentiment of the reviews.

<ul>

<li>Positive </li>
<li>Neutral </li>
<li>Negative </li>
</ul>

</p>
<h1> NLTK </h1>
<p>

On the first approach I used NLTK to tokenize the words and to do the preprocessing part of the text and feature engineering (word embedding).

I imported the VADER algorithm, which is a lexicon and rule-based model, that takes into account the polarity of the emotion, positive or negative, and the strenght of the emotion.

Despite that, since it's a bag of words like approach, it doesn't see the words based on their context.

</p>
<h1> TF-IDF </h1>

<p>
TF-IDF is another method to transform words into vectors that the computer can read.

It's an evolution of the bag of words method, where it uses frequency that the word appeared on a certain text compared to the frequency it appeared on the whole dataset.

![TF-IDF FORMULA](/assets/tfidf.png)

</p>

<h1> BERT </h1>

<p>

BERT is a very interesing method. <br>
 In normal word2vec using continous bag of words, we try to predict the word from it's context and with Skip Gram we try to predict the context with the word. The problem with this approach, is that the embedding is fixec. <br>
  Which means it doesn't look at the context where the word is, but just at the word. <br>
  
  For example: <br>
  
 <ul>
   <li> This judgment was not <b>fair</b></li>
   <li> This <b>fair</b> was amazing!!</li>
 </ul> 

 
  Word2vec would categorize or represent both words with very similiar vectors. But we know that despite being the same word, the meaning is totally different.<br><br>
  That's where BERT - Bidirectional Encoder for Transfomers, comes into play.<br>
     
  BERT looks into the context of the word. In the case of the above example, the vectors would be different.
</p>

<h1> Conclusion </h1>

We could see that despite the flaws of the bag of words methods, the model could categorize the sentiment of most reviews correctly. But as we would expect, there was a lot of uncertainty regarding that. <br>

For TF-IDF it had a bit less uncertainty, but there wasn't much improvement. Trying new classification methods may change the result. <br>

Unfortunately, I couldn't run BERT model on the dataset since it' too big and CPU can't handle it. But if everything goes well, BERT should be a much more robust method than those we tried. <br>

Overall, there is quite a bit of things I can try and see if I can improve the results and the data visualization. <br>

Thank you for reading and have a nice week!!! <br>

<h1> References</h1>

<p>
  
</p>
