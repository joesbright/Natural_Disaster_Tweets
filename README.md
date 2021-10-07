# Natural Language Processing with Disaster Tweets

This repository contains my submissions to the Kaggle Natural Language Processing with Disaster Tweets. Each notebook will have a filename like <pre><code>natural_disaster_METHOD</code></pre> where METHOD details how the classifcations were performed. E.g. <code>natural_disaster_tfif</code></pre> contains my competition submission using term frequency–inverse document frequency (tfidf).

## Term Frequency-Inverse Document Frequency

Term frequenct-inverse document frequency is a statistic that combines the concept of term frequency and inverse document frequency. Term frequency (assuming logarithmic normalisation) is given by <a href="https://www.codecogs.com/eqnedit.php?latex=tf(w,d)=(1&plus;log(f(w,d)))" target="_blank"><img src="https://latex.codecogs.com/gif.latex?tf(w,d)=(1&plus;log(f(w,d)))" title="tf(w,d)=(1+log(f(w,d)))" /></a> where
