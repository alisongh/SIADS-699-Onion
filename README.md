# Team Onion
## SIADS 699 Capstone, University of Michigan, Ann Arbor
### Subject: Identifying accurate news vs fake news/misinformation vs satirical news

Team members: Christine Gregg, Liwen Alison Huang, Ali Tobah 

**Question:**
* Can a model be trained to differentiate fake news from real news based on the language and topic of the article?
* If a model does well at differentiating between real and fake news, does it also perform well at differentiating between fake news and satire?

**Datasets**
* Fake News vs Satire
  - Paper: https://dl.acm.org/doi/10.1145/3201064.3201100
  - Dataset: https://github.com/jgolbeck/fakenews
* Real News vs Fake News
  - Dataset: https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset?select=True.csv
* Real News vs Satire
  - Paper: https://aclanthology.org/D17-1211/
  - Dataset: https://data.mendeley.com/v1/datasets/hx3rzw5dwt/draft

These are publicly accessible datasets. In general, they include texts of news articles labeled as 'fake', 'satire' or 'true'. One dataset matches the fake news to rebuttals or satire.

**Minimum viable product (MVP)**
* Alongside our final report, we will include a faceted bar plot showing the counts of true positives, false positives, true negatives, and false negatives for each news type (real, fake, and satire). We will also include a table of performance metrics (most notably, the F1 score).
* Additional possibilities we might explore for model explainability:
  - SHAP （SHapley Additive exPlanations） https://shap.readthedocs.io/en/latest/index.html 
  - https://towardsdatascience.com/lime-vs-shap-which-is-better-for-explaining-machine-learning-models-d68d8290bb16 

**Ethical Considerations and Limitations**
* The potential harm of mislabeling news as real, fake, satire
* Potential to propagate biases/stereotypes
* Insufficient representation of certain groups (using mainstream news sources as training data - not all racial/ethnic groups use similar language)
* Insufficient resources of news (all resources are written in English, and most models are designed for English-written news. Since text mining and analysis involves a significant language component, an ideal ML model can be applied for multilingual news articles)

**Technical Challenges**
* Text analysis of full news articles could take a while to run - optimizing code will be important
* Current limitations in the literature - this is an ongoing area of research
* It is possible that we will not have enough labeled satirical data and/or that satirical articles will skew towards certain topics.

