# Natural Language Processing with Disaster Tweets

This repository contains my submissions to the Kaggle Natural Language Processing with Disaster Tweets. Each notebook will have a filename like <pre><code>natural_disaster_METHOD</code></pre> where METHOD details how the classifcations were performed. E.g. <code>natural_disaster_tfif</code></pre> contains my competition submission using term frequency–inverse document frequency (tfidf).

## Term Frequency-Inverse Document Frequency

Term frequenct-inverse document frequency is a statistic that combines the concept of term frequency and inverse document frequency. Term frequency (assuming logarithmic normalisation) is given by <img src="https://latex.codecogs.com/gif.latex?%5Cbg_white%20tf(w,d)=(1&plus;log(f(w,d)))" title="tf(w,d)=(1+log(f(w,d)))"/> where tf is the term frequency, which is a function of w (a word) and d (the specific document in the document set you are considering (D), while f is the raw count of word w. A word that doesn't appear in the document will have a tf value of zero. The score increases logarithmically with the raw count. The tf varies between documents and words.

The inverse document frequency of a word quantifies how common it is accross the set of documents. It is given by <img src="https://latex.codecogs.com/gif.latex?%5Cbg_white%20log(\frac{N_{D}}{N_{w}+1})"/>, where N_D is the number of documents and N_w is the number of times the word appears in all documents. The idf is constant for a given word between documents. 

Simply multiplying these terms gives the term frequency-inverse document frequency. This acts to suppress words that occur at high frequency if they also appear in many documents (i.e. does a good job at filtering out common words like "the" which will have a low idf score. 
