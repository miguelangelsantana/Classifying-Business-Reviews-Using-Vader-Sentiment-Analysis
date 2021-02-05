# Movie Review Text Classification
## Classifying Positive and Negative Review with NLP

* **Author**: Miguel Santana

Thank you for reviewing this repository. The author's contact info, sources and social media profiles are listed below under **further information.**

Thank you for reviewing this repository. The author's contact info, sources and social media profiles are listed below under further information.

The contents of this repository detail an analysis of two text files: Amazon product reviews and movie reviews. The movie review file is similar to the one used in the github project **Text Classification - Movie Reviews.** The file was used in order to compare text versus sentiment classification.

For illustrative purposes, text has been preprocessed and the labels are provided in order to assess model performance. The analysis will provide insight into method's used by NLP professionals to evaluate text for businesses.

### Project Framework

![!](/images/OSEMN.png)

**Data processing and analysis is completed using the OSEMN framework. The structure includes: Obtaining the data, Scrubbing (processing), Exploratory Data Analysis, Statistical Modeling and Interpretation of the Results.**

### The Data

The movie review dataset is originally sourced from Stanford Artificial Intelligence Laboratory (SAIL) but was provided via Udemy. The Amazon text file was also provided via the same course. The Udemy citation is available below under **sources.** Please visit [ai.stanford.edu](http://ai.stanford.edu/~amaas/data/sentiment/) for more information on the movie review dataset. 

## Scrubbing/Data Cleaning 

**Key Decisions**

* Address whitespace strings
* Drop null values

## Vader Sentiment Analysis | Raw Text

Valence Aware Dictionary for Sentiment Reasoning is a model used for text sentiment analysis in natural language processing. The model offers insight into polarity as well as intensity, referring to positive, neutral, negative and by how much.

## Amazon Reviews

#### Exploratory Data Analysis 
**Length of Reviews**

![!](/images/amazonlength.jpg)

### Vader Results | Amazon


                  precision    recall  f1-score   support
    
             neg       0.86      0.51      0.64      5097
             pos       0.64      0.91      0.75      4903
    
        accuracy                           0.71     10000
       macro avg       0.75      0.71      0.70     10000
    weighted avg       0.75      0.71      0.70     10000
    
    
    
    There overall accuracy score is 0.7091.


## Movie Reviews

#### Exploratory Data Analysis 
**Length of Reviews**

![!](/images/movielength.jpg)

### Vader Results | Movie Reviews


                  precision    recall  f1-score   support
    
             neg       0.72      0.44      0.55       969
             pos       0.60      0.83      0.70       969
    
        accuracy                           0.64      1938
       macro avg       0.66      0.64      0.62      1938
    weighted avg       0.66      0.64      0.62      1938
    
    
    
    There overall accuracy score is 0.6367389060887513.


## Interpreting Results 

The Vader sentiment analyzer was unable to out perform the text classifier but it offered insight into advancements in natural language processing. Keep in mind, Vader processed the raw text and offered respectable performance despite a lack of train test split or parameter tuning. Human semantics can be tricky and I look forward to continued advancements in sentiment analysis with respect to natural language processing. 

### Future Work

Future work should include web scraping of additional sources to get a broader view of Vader's performance across multiple disciplines and industries. In future projects, speech-to-text in combination with text classification should be applied to larger and more robust data sets in order to evaluate performance on real business cases.  

#### Further Information

Please review the narrative of our analysis in [our jupyter notebook](./jupyter_notebook.ipynb) or review our [presentation](/powerpoint/powerpoint.pdf)

For any additional questions, please reach out via email at santana2.miguel@gmail.com, on [LinkedIn](https://www.linkedin.com/in/miguel-angel-santana-ii-mba-51467276/) or on [Twitter.](https://twitter.com/msantana_ds)

#### Sources

Additional analysis, notes and file sources can be found on Udemy. 

* Course Name: NLP - Natural Language Processing | Jose Portilla

##### Repository Structure:

```

├── README.md               <- The top-level README for reviewers of this project.
├── jupyter_notebook.ipynb     <- narrative documentation of analysis in jupyter notebook
├── presentation.pdf        <- pdf version of project presentation

```

