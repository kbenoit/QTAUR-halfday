Advanced analysis using quanteda
========================================================
author: Ken Benoit
date: 2017-11-15
autosize: true
css: custom.css
font-family: arial






Advanced analysis using quanteda
================================

**quanteda** has the following advanced functionality:

* extensive weighting functions, such as _tf-idf_
* extensive feature selection options, using fixed matching, "glob" matching, and regular expression matching
* ability to constuct a feature co-occurrence matrix, including weighted variations 
    - for input to _word2vec_, **text2vec**, etc.

"textual statistics" functions
==============================

name               | function
-------------------|-----------------
`textstat_collocations` |	calculate collocation statistics
`textstat_dist` |	distance computation between documents or features
`textstat_keyness` |	calculate keyness statistics
`textstat_lexdiv` |	calculate lexical diversity
`textstat_readability` |	calculate readability
`textstat_simil` |	similarity computation between documents or features

"text model" functions
======================

name               | function
-------------------|-----------------
`textmodel_ca` |	correspondence analysis of a document-feature matrix
`textmodel_nb` |	Naive Bayes (multinomial, Bernoulli) classifier for texts
`textmodel_wordfish` | Slapin and Proksch (2008) text scaling model
`textmodel_wordscores` |	Laver, Benoit and Garry (2003) text scaling
`textmodel_wordshoal`	| Lauderdale and Herzog (2017) text scaling model
`textmodel_affinity`	| (coming soon) Perry and Benoit (2017) class affinity scaling
`coef.textmodel` | extract coefficients from a `textmodel`

text plotting functions
=======================

name               | function
-------------------|-----------------
`textplot_scale1d` |	plot a fitted scaling model
`textplot_wordcloud` |	plot features as a wordcloud
`textplot_xray` |	plot the dispersion of key word(s)
`textplot_keyness` | plot association of words with target v. reference set

works very well with other packages
===================================

* `convert()` will transform a **quanteda** `dfm` into any number of "foreign" formats
* can convert to and from the "tidy" format of the **tidytext** package


works well with spacyr
==========================

* the R package **spacyr** provides an interface to the Python module [spaCy](spacy.io)
* part of speech tagging and dependency parsing in 6+ languages
* super fast

====


























```
Error in spacy_initialize() : 
  spaCy or language model en is not installed in any of python executables.
```
