![Picture2](https://user-images.githubusercontent.com/45460506/103392391-42949f00-4ae3-11eb-959f-edc4c7fdd742.png)
# NLP-on-scientific-articles-for-information-retrieval
This experiment will work on language modeling to provide a way of giving a token of identification to research articles which facilitates recommendation and search process.

Key work on this experiment is **word embedding**. I will test several wording embedding methods such as TF-IDF and word2vec. And then, I will evaluate the classification modeling performance on vectors from different word embedding. The best word embedding should be able to reasonably separate the articles and give out the best classification prediction. I will use the best word embedding method to realize information retrieval and produce a web APP for [Scientific-articles-search](https://scientific-articles-search.anvil.app/).

## [Presentation](https://github.com/zhaoxin1124ds/NLP-on-scientific-articles-for-information-retrieval/blob/main/NLP_information_retrieval.pdf)
https://github.com/zhaoxin1124ds/NLP-on-scientific-articles-for-information-retrieval/blob/main/NLP_information_retrieval.pdf

## Data
The data is from [Kaggle](https://www.kaggle.com/vetrirah/janatahack-independence-day-2020-ml-hackathon) and contains abstract and title for a set of scientific papers. All the papers have been labeled according to 6 topics: computer science, physics, mathematics, statistics, quantitative biology, and quantitative finance.

## Experiment procedure
#### Data pre-processing
I removed the numbers, puntuations, extra white space, new lines, etc.
#### Word embedding and classification
I will test below word embedding algorithms:
* TF-IDF
* word2vec
* Since the document is labeled, I will acquire classification score to evaluate difference vector space models
#### Information retrieval
I will use cosine similarity ranking to realize the information retrieval

## Results
* The classification accuracy score is 0.84
* The product of information retrieval returns reasonable recommendations for anu queries

## More thinks for further improvement
* Larger documents to improve the balance
* Playing with weight between the title and abstract
* BERT for a more advanced word embedding attempt

