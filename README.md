# Quantitative Text Analysis Using R: A Half-Day Tutorial

[Kenneth Benoit](kbenoit@lse.ac.uk), Department of Methodology, LSE  
[Kohei Watanabe](K.Watanabe1@lse.ac.uk), Department of Methodology, LSE  

**Version:** 15 November 2017

----

This repository contains the workshop materials for a half-day tutorial *Quantitative to Text Analysis Using R*.  This project was supported through European Research Council grant ERC-2011-StG 283794-QUANTESS.

## Instructions for using this resource

You have three options for downloading the course material found on this page:  

1.  You can download the materials by clicking on each link.  

2.  You can "clone" this repository, using the buttons found to the right side of your browser window as you view this repository.  This is the button labelled "Clone in Desktop".  If you do not have a git client installed on your system, you will need to [get one here](https://git-scm.com/download/gui) and also to make sure that [git is installed](https://git-scm.com/downloads).  This is preferred, since you can refresh your clone as new content gets pushed to the course repository.  (And new material will get actively pushed to the course repository at least once per day as this course takes place.)

3.  Statically, you can choose the button on the right marked "Download zip" which will download the entire repository as a zip file.

You can also subscribe to the repository if you have [a GitHub account](https://github.com), which will send you updates each time new changes are pushed to the repository.

## Objectives

This workshop covers how to perform common text analysis and natural language processing tasks using R.  When used properly, R is a fast and powerful tool for managing even very large text analysis tasks.  

The course consists of instructor presentations in three sets, followed by interactive exercises that students are meant to work through during the workshop.

We will cover how to format and input source texts, how to structure their metadata, and how to prepare them for analysis.  This includes common tasks such as tokenisation, including constructing ngrams and "skip-grams", removing stopwords, stemming words, and other forms of feature selection.  We show how to: get summary statistics from text, search for and analyse keywords and phrases, analyse text for lexical diversity and readability,  detect collocations, apply dictionaries, and measure term and document associations using distance measures.  Our analysis covers basic text-related data processing in the R base language, but most relies on the [**quanteda**](http://quanteda.io) package for the quantitative analysis of textual data.  We also discuss (briefly) how to pass the structured objects from **quanteda** into other text analytic packages for doing topic modelling, latent semantic analysis, regression models, and other forms of machine learning.


## Prerequisites

While it is designed for those who have used R in some form previously, expertise in R is not required, and even those with no previous knowledge of R are welcome.


## Part 1: Getting Started and Basic Text Analysis

*  An [overview of the **quanteda** package](overview/quanteda_overview.md)
*  [Getting started, text import, and basic analysis](1_getting_started/1_getting_started.md)
*  Some basic **quanteda** [workflow](1_getting_started/workflow.md) guidelines

### Interactive

Setting up RStudio and **quanteda**:  

*  [CRAN](https://cran.r-project.org) for downloading and installing R
*  **Configuration test:**  Try running this RMarkdown file: [test_setup.Rmd](1_getting_started/test_setup.Rmd).  If it builds without error and looks like [this](https://rawgit.com/kbenoit/QTAUR-halfday/master/1_getting_started/test_setup.html), then you have successfully configured your system.  

Step through a simple analysis:  
*  Step through execution of the [1_getting_started/1_getting_started.Rmd](1_getting_started/1_getting_started.Rmd) file.  (This requires that you use RStudio and have installed the **knitr** and **rmarkdown** packages, but if you try to click the "Knit" button and have not yet installed these, the program will prompt you to do so.)
*  Sample data files: 
    *  [SOTU_metadata.csv](https://github.com/kbenoit/QTAUR-halfday/blob/master/data/SOTU_metadata.csv)  
    *  [inaugTexts.csv](https://github.com/kbenoit/QTAUR-halfday/blob/master/data/inaugTexts.csv)  
    *  [tweetSample.RData](https://github.com/kbenoit/QTAUR-halfday/blob/master/data/tweetSample.RData)

## Part 2: Basic text analysis using collocation, keyness and dictionary

*  [Basic analysis of texts](https://rawgit.com/kbenoit/QTAUR-halfday/master/2_basic/2_basic.html)

## Part 3: Advanced analysis and working with other text packages

*  [Advanced analysis and working with other packages](3_advanced/03_advanced.md)
*  [as slides](https://rawgit.com/kbenoit/QTAUR-halfday/master/3_advanced/advanced_rpus.html)
*  **Twitter analysis example**, and the instructions for setting up your own Twitter app, in [Twitter.Rmd](3_advanced/Twitter.Rmd). 

### Interactive: Step through execution of the [.Rmd file](3_advanced/advanced.Rmd)



## More resources

### Extension packages

*  [**spacyr**](https://github.com/kbenoit/spacyr): part-of-speech tagging and dependency parsing using the [spaCy](http://spacy.io) engine.  
*  [**LIWCalike**](https://github.com/kbenoit/LIWCalike): replicate the Linguistic Inquiry and Word Count program's functionality.  
*  [**readtext**](https://github.com/kbenoit/readtext):  read texts into R (replaces the `textfile()` function from **quanteda**).  
*  [**preText**](http://cran.r-project.org/package=preText):  Diagnostics to assess the effects of text "pre-processing" decisions.

### Additional leadning resources

Designed to be done before the course or after, to augment what is presented during the course.  These are just suggestions -- no reading for the course is required.

*  [Sanchez, G. 2013. Handling and Processing Strings in R Trowchez Editions. Berkeley, 2013.](http://www.gastonsanchez.com/Handling and Processing Strings in R.pdf)  
*  [**stringi** package page](http://www.rexamine.com/resources/stringi/), which also includes a good discussion of the [ICU library](http://site.icu-project.org)
*  Some guides to regular expressions: [Zytrax.com's User Guide](http://www.zytrax.com/tech/web/regex.htm)
 or the comprehensive resources from http://www.regular-expressions.info  
*  See the [`quanteda` tag on Stack Overflow](http://stackoverflow.com/questions/tagged/quanteda), where you can pose questions and see some brilliant answers by our development team.
