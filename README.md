# Web-scraping Poe's poems and performing emotional analysis

This repository contains a filled Jupyter Notebook file with the full code and results of web-scraping Edgar Allan Poe's poem collection using [Beautiful Soup 4](https://www.crummy.com/software/BeautifulSoup/bs4/doc/) and performing sentiment analysis on them through [Vader's Sentiment Analyzer](https://github.com/cjhutto/vaderSentiment) and [DepecheMood's Lexicon](https://arxiv.org/abs/1405.1605). All code inside of it is mine and was submitted to a midterm evaluation.

The file `requirements.txt` contains all the modules required to run the Jupyter Notebook. Pip can be used to install them with the `pip install -r /path/to/requirements.txt` command.

## Tasks performed

Below are the several tasks that are performed by the notebook

1. **Web-scraping**: web-scrapes Edgar Allan Poe's poem collection from [The Project Gutenberg](https://www.gutenberg.org/files/10031/10031-h/10031-h.htm) into a JSON file (shown in the repository).
2. **Compiles [DepecheMood's Lexicon](https://arxiv.org/abs/1405.1605)**: compiles the lexicon provided by DepecheMood into a usable data structure to determine the emotions that each word carries.
3. **Parses poems and performs sentiment analysis**: tokenizes each poem into stanzas and words using [NLTK's Punkt tokenizer](https://www.nltk.org/_modules/nltk/tokenize/punkt.html) and then plugs them into the lexicon and vader's analyzer to obtain their sentiment.
4. **Creates a Zeitgeist of the whole collection**: using the generated data, an averaged "zeitgeist" (the sentiment) of the collection as a whole is created.
5. **Plots pie charts to show the summary**: using matplotlib.
