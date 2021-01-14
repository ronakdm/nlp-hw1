# nlp-hw1
Homework 1 for Natural Language Processing. Contains code for implementing a sentiment lexicon-based classifier and logistic regression on the Pang and Lee movie review dataset.

## Data
Two datasets are needed:
- Pang and Lee movie review data, which can be downloaded from http://www.cs.cornell.edu/people/pabo/movie-review-data/ by clicking the "polarity dataset v2.0" link.
- The Bing Liu sentiment lexicon, which can be downloaded from https://www.cs.uic.edu/~liub/FBS/sentiment-analysis.html#lexicon by clicking the "A list of English positive and negative opinion words or sentiment words " link.
The code assumes that the downloaded files are unarchived, and available in the following hierarchy, placed in the same directory as `hw1_1.ipynb1`.

**Movie Review Data:**
```
├─── poldata.README.2.0
├─── txt_sentoken/
│ ├─── pos/ cv999_13106.txt, cv998_14111.txt, ...
│ ├─── neg/ cv999_14636.txt, cv998_15691.txt, ...
```

**Sentiment Lexison:**
```
opinion-lexicon-English/
├─── positive-words.txt
├─── negative-words.txt
```

## System Requirements

The code is written in Python 3.7, and depends only on `numpy` and built-in modules `glob` and `pickle`. An environemtn with `jupyter` is required.

## Intructions

To reproduce the results, open `hw1_1.ipynb` in Jupyter, and run every cell. There are markdown cells that explain key steps, such as preprocessing, featurization, optimization, and metrics. 
With `np.random.seed(517)`, you should observe an accuracy and F1 score of about `0.74` for unregularization logistic regression, and accuracy and F1 score at about `0.69` for the lexicon-based classifier.
