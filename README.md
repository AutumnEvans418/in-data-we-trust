# Team In Data We Trust: Topic Modeling
Final Project Submission to perform topic modeling on NYT articles dataset.

# Problem
**Topic Modeling:**
Introduction: In the world we live in, data streams are constantly being gathered. This means that mining the gathered data for insights might get extremely laborious and time-consuming. Large amounts of textual data may be arranged, searched for, and understood with the help of topic modeling. In the field of machine learning, a topic model is precisely described as a natural language processing method that uncovers text's latent semantic patterns inside a corpus, or collection of documents. A continuous set of words, such as a paragraph or an article, where each article has a set of words, is generally referred to as a document.

**Task**: Perform the topic modeling on the dataset below and retrieve the most important topics. Also report on the key words associated with each topic.
Data Link: https://www.kaggle.com/datasets/tumanovalexander/nyt-articles-data

## Context
The dataset was downloaded for one of the hackathons, in which the task was to determine the sentiment of the news.

## Content
There are a year of publishing, title and an excerpt from the news in the columns "year", "title", "excerpt".

Data provided by The New York Times https://developer.nytimes.com/

# Topic Modeling Process
Below are the steps we will perform:
## Discovery
1. Determine the structure of the data and the scope.
1. Evaluate data completeness.
## Cleaning
1. Clean up the data by removing missing values and duplicates. - **Autumn**
1. Convert titles + excerpts to lower case. - **Autumn**
1. Remove punctuation. - **Autumn**
1. Tokenize words. - **Joel**
1. Remove stop words. - **Joel**
1. Lemmatization/Stemming - **Joel**
1. Create a Term-Document-Matrix - ?

### Cleaning Result
|Title_Excerpt|Words|
|---|---|
|Title<br>Some excerpt.|[title, some, excerpt]|

The table above will be converted into the TDM below:

Term-Document-Matrix (TDM):

|Term|Title_Excerpt1|Title_Excerpt2|
|---|---|---|
|title|1|0|
|some|0|2|

## Analysis: Latent Dirichlet Allocation (LDA)
In order to work on this in parallel, we will create a standard function:
```python
def lda(input, num_topics): #input=[(0,1),(1,2)]
    #train model
    pass

```

- Train the LDA model. - **Manan**
- Fine tune the LDA model (selecting optimal number of topics for the dataset). - ?
- Generate diagrams for each topic, displaying the top terms for each topic. - ?

# Running the Project
1. Clone the git repo.
1. Due to the significant size, the data isn't stored along with the source code. You will need to download the dataset. [See docs here](src/raw_data/README.md)
1. Install python 3.13.5. We used https://github.com/pyenv-win/pyenv-win to manage our python versions.
1. Run `pip install -r .\requirements.txt` to install the necessary packages.