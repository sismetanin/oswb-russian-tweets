# Observable Subjective Well-Being Inferred from Tweets in Russian

This repo contains code for measuring Observable Subjective Well-Being based on tweets in Russian.

## Twitter Data
We used the Twitter Stream Grab[^1] as a data source of tweets in Russian. Twitter Stream Grab is a publicly available historical collection of JSON grabbed from the general Twitter “Spritzer” API stream.

## Sentiment Classification Model
We fine-tuned RuRoBERTa-Large[^rbrt] on RuSentiTweet[^rusentitweet] and achibed new state-of-the-art results of macro $F_1=0.7229$ and weighted $F_1=0.7281$, surpassing the previous SOTA results achieved by the RuBERT model.

## Subjective Well-Being Data
We used survey-based VCIOM Happiness Index[^vciom], which is regularly reported by Russia Public Opinion Research Center.

[^1]: https://archive.org/details/twitterstream
[^rbrt]: https://huggingface.co/sberbank-ai/ruRoberta-large
[^rusentitweet]: https://peerj.com/articles/cs-1039/
[^vciom]: https://wciom.ru/analytical-reviews/analiticheskii-obzor/indeks-schastja
