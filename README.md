# Geographic named entity recognition 

Original idea: explore neighborhood level relationship between sentiment in articles and common metrics of neighborhood change (eg income levels, land prices)

## Analysis steps
1. Assign articles to a location
  - Can we identify if the article is about a specific neighborhood? more than one?
2. Analyze sentiment of articles
  - again likely to be a mix of positive/negative sentiments in a given article, will need way to categorize - eg maybe percent of positive/negative/neutral sentences
3. Collect articles from multiple years
  - if possible likely start with articles around 2000 and 2010 to use full Census as basis of change metrics
4. Gather neighborhood change metrics
  - start with Decennial Census
  - if have articles from more than ~2-3 years probably use LODES to have geographically granular and consistent measure of annual data

## Other notes
1. Focus on New York City and neighborhoods.

Possible approach: using "neuralcoref" which finds mentions of named entities throughtout the text. Sample code uploaded - mentions.py.

Next step: run this on corpus. Use existing corpus or create one using Google News API.

NLTK Gazeetteer - cities and countries

## sources
Should all be cited in various notebooks/etc in this repo, but here are some articles/sources helpful in exploring this idea
1. Susan Li's Named Entity Recognition series: 
  - https://towardsdatascience.com/named-entity-recognition-with-nltk-and-spacy-8c4a7d88e7da
  - https://towardsdatascience.com/named-entity-recognition-and-classification-with-scikit-learn-f05372f07ba2
2. Stackoverflow is always useful.
  - https://stackoverflow.com/questions/30150047/find-all-locations-cities-places-in-a-text