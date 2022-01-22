# AmazonReviewAnalysis - A Natural Language Processing Web App
** CURRENT WORKING BRANCH: ver6 **


Tech Stack
---
- Django: backend
- React.js: frontend
- Charts.js: data visualization
- selenium: data scraper
- nltk/spacy: natural language processing
- sklearn: machine learning


Members
---


Approach
---
- Use TFIDF to assess how relevant a keyword is with respect to the 5-star review set.
- Use Count Vectorizer to see how many times a keyword appears in a 5-star review set.
- Use LDA to find the common topics
- Visualize the data in a web app

Task description:
---
- Task description: we are provided with a product on Amazon (in this project we have Starbucks Frappuccino), and we have to analyse the product's reviews and extract information that might be useful for our client to implement to their product of the same category.
- Motivation: this project hopes to assist retailers in understanding better about what makes a bestseller and about their competitors' products, providing them with a tool to better make decisions about different approaches to maximize their chances of being among the top-selling.


Survey
---
1. Existing methods for the task: 
- CountVectorizer: this simple technique only provides us with a word-document matrix, i.e. the final output would be a list of words and the number of times they appear in the entire review set. Therefore, it is useful for preprocessing, but not so much useful information could be obtained from CountVectorizer.
- TFIDF: a very popular method to list out significant words in the review set. TF-IDF not only takes into account how many times a word appear in the document (a review in this case), but also putting a restraint on those words that are frequently used. This method goes by the following formula:

```
tf-idf(t, d) = tf(t, d) * idf(t)

where:
tf(t,d) = count of term t in document d / number of words in d
idf(t) = log_e(N/ df(t))
N = Number of documents
df(t) = Document frequency of a term t
```	


Demo
---
1. Data Visualization

![image](https://user-images.githubusercontent.com/47298653/148825435-5a590bee-013d-4b09-9bc5-bb601310774d.png)

![image](https://user-images.githubusercontent.com/47298653/148825489-45e1935b-31d5-4382-a466-f0f4208dc634.png)



