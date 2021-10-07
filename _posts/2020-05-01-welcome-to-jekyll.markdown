---
layout: post
title:  "Paper: Modeling Movement: A machine-learning approach to track migration routes after displacement"
date:   2021-09-20 12:09:11 +0200
category: Paper-Reviews
---
([Paper
link](https://d1wqtxts1xzle7.cloudfront.net/63726782/Predicting_Forced_Population_Displacemen-with-cover-page-v2.pdf?Expires=1633610854&Signature=Ont1e6RFJ6LIYHvfH3S3laZbmGIXuLPAh30q18EntO2ASjHvGXp6k~GvfW-iujUPwCeHkovCTeei7QxNd28Hge7LyjOBpawc~AFcfSOIsmweauX2DsBtfYyJOOcw1WX4GUCbYcdobBZfWfx5djFo33AO9qGz9kavAQdCcz4NQzPExLXdvagKFMbpepN5Hf8JfqOlyhj0MKYbdAWDvbaZvs7ELnBVAZCQ1xkPK1Dt4WVpPPsazQXBYWLNVNHLlOydg1gwPFEiJFYcIrlPqa8hZd4AzuZE1AT2P56qiEfeq7MbcSFhZeafpVlCqsNoouwb6NR-T~hxjNG9GVqx-b7BlA__&Key-Pair-Id=APKAJLOHF5GGSLRBV4ZA))

This paper introduces a model for extracting levels of local violence by identifying violent terminology in news articles. The idea being that
violence in a region is one of the driving factors for causing forced displacement. They use time-sensitive topic modeling.

## Key Pieces

### Non-negative matrix factorisation (NMF)

Matrix $V$ with documents as columns and words as rows where the elements are the frequency of the word in the document. This can be factorised into:

$$V=WH$$

with, for the jth document and kth topic:

$$V(:,j) \approx \sum^r_{k=1}W(:,k) H(k,j)$$

Each document (column in $V$) can be considered formed from a set of topics, $r$,. $W$ is a features matrix assigning words to hidden topics, $k$. $H$
is a weights matrix assigning topics to documents. The number of topics is a key pre-defined measure and is optimised using semantic analysis on the
topics.












### LDA (Latent Dirichlet Allocation) ([TDS article](https://towardsdatascience.com/latent-dirichlet-allocation-lda-9d1cd064ffa2)).
 This is a method for grouping words into a (pre-defined) number of (not defined) topics. The documents are represented as groups of topics.

The method is to:
 > - Randomly assign words in the dataset to a topic 
 > - Calculate the proportion of words in a document that are assigned to a given topic $$P(word\|topic)$$
 > - Calculate the proportion of documents containing a word that are assigned to a topic $$P(topic\|document)$$
 > - Calculate the probability that a word is associated with a given topic $$P(word\|topic)$$ = $$P(topic\|document) \times P(word\|topic)$$


