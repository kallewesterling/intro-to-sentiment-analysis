# Install NLTK

## Step 1: Install NLTK

If you're on a Mac or UNIX machine, you should just be able to run the following command:

```sh
$ pip install --user -U nltk
```

If you have trouble with the installation (or you're on a Windows machine), see the [Official Installation Instructions for NLTK](https://www.nltk.org/install.html).

## Making sure everything is installed

In order to make sure everything is installed, first let's check that NLTK was fully installed. This should give you no message:

```python
import nltk
```

Now let's make sure that the `vader_lexicon` is installed:

```python
if nltk.download('vader_lexicon', quiet=True): print("You're good to go!")
```

This should generate a message `You're good to go!` If it does not, you need to troubleshoot.

Now all we need to do is to import the actual VADER analyzer.

```python
from nltk.sentiment.vader import SentimentIntensityAnalyzer
```

----

Hutto, C.J. & Gilbert, E.E. (2014). VADER: A Parsimonious Rule-based Model for Sentiment Analysis of Social Media Text. Eighth International Conference on Weblogs and Social Media (ICWSM-14). Ann Arbor, MI, June 2014.
