# Support Ticket Classification - FUTURE_ML_02

So this was my second task and it was honestly more interesting than
I expected. The idea was to automatically classify customer support
tickets and tag them with priority levels like high medium or low.

## What I did

First thing was cleaning the messy ticket text. Lot of noise in there
like punctuation random symbols and stopwords. Used NLTK to tokenize
everything and get it into a usable format. That alone took quite some
time to get right.

Then converted the cleaned text into numbers using TF-IDF and trained
a Naive Bayes classifier to sort tickets into categories like billing
technical account and general issues.

Also wrote a small priority tagging logic based on keywords. If someone
wrote urgent or not working or refund it would flag it as high priority.
Pretty simple but actually works well in practice.

## What I used

- Python and Jupyter Notebook
- NLTK for cleaning and tokenization
- Scikit-learn for the classifier
- Matplotlib and Seaborn for charts
- WordCloud to visualize common words

## What I learned

- Text data is way messier than normal tabular data
- TF-IDF is super useful for converting text to features
- Priority logic does not need to be complex to be effective
- Confusion matrix really helps understand where model goes wrong

## Dataset

Used a publicly available customer support ticket dataset.

## Result

The classifier worked pretty well overall. Word clouds per category
looked really cool and the confusion matrix showed most tickets were
being classified correctly. Definitely one of the more practical tasks
I have done so far.
