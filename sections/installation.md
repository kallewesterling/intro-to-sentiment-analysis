## Making sure everything is installed

In order to make sure everything is installed, first let's import nltk. This should give you no message:

```python
import nltk
```

Now let's make sure that the `vader_lexicon` is installed:

```python
if nltk.download('vader_lexicon', quiet=True): print("You're good to go!")
```

This should generate a message `You're good to go!` If it does not, you need to troubleshoot.

Now all we need to do is to import the actual VADER analyzer.

Based on:
- Hutto, C.J. & Gilbert, E.E. (2014). VADER: A Parsimonious Rule-based Model for Sentiment Analysis of Social Media Text. Eighth International Conference on Weblogs and Social Media (ICWSM-14). Ann Arbor, MI, June 2014.

```python
from nltk.sentiment.vader import SentimentIntensityAnalyzer
```
