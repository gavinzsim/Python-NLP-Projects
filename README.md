# Python NLP Projects

This repo has some of my LING 380 projects/assignments as an exploration of NLP tools. They are both Jupyter notebooks and mostly focus on using Python tools to look at and classify text.

One notebook, [`Text Analysis.ipynb`](./Text%20Analysis.ipynb), compares a surgery textbook, a Sherlock Holmes story, and a movie script. I took a closer look at things like word counts, lexical diversity, common words, and named entities to see how the genres differ.

The other, [`Sentiment Classification with Feature Importance.ipynb`](./Sentiment%20Classification%20with%20Feature%20Importance.ipynb), is a movie-review sentiment classifier. It cleans and stems the reviews, trains a random forest model, then shows the confusion matrix and which words were most significant to the model.

## Tools used

The notebooks use Jupyter, NLTK, pandas, NumPy, scikit-learn, spaCy, matplotlib, and seaborn.

To run them locally:

```bash
pip install jupyter nltk pandas numpy scikit-learn spacy matplotlib seaborn
python -m nltk.downloader punkt punkt_tab stopwords vader_lexicon
python -m spacy download en_core_web_sm
jupyter notebook
```

Then open the notebook you want to look at and run the cells in order.

## Data

The notebooks are included here, but the original text data is not. You will need to add compatible files before running them:

- `Text Analysis.ipynb` expects `.txt` files in `./data`.
- `Sentiment Classification with Feature Importance.ipynb` expects positive and negative review files in `./pos` and `./neg`.



