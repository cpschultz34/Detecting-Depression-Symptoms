# Detecting-Depression-Symptoms
This project implements the major pieces of the paper “Detecting Symptoms of Depression on Reddit” by Liu et al. In it, I take raw data from reddit users in various subreddits (both depression-related and unrelated) and split these into symptoms of depression posts and control posts based on the paper's implementation. I then tokenize and process the posts and use them to train a Latent Dirichlet Allocation (LDA) model. I use this LDA model as well as a DistilRoBERTa model to extract probability distributions over topics and token embeddings per post, respectively. I use these to train a Random Forest Classifier with 5-fold cross-validation to compare AUC scores across models for each depression symptom. My results are at the end of the Jupyter Notebook.

### Link to video overview
https://drive.google.com/file/d/1wRVrcZ3k7UPb34RS1ewH1pE2-yh3pB-F/view?usp=sharing

### Reference Paper
Tingting Liu, Devansh Jain, Shivani R Rapole, Brenda Curtis, Johannes C. Eichstaedt, Lyle H. Ungar, and Sharath Chandra Guntuku. 2023. Detecting Symptoms of Depression on Reddit. In Proceedings of the 15th ACM Web Science Conference 2023 (WebSci '23). Association for Computing Machinery, New York, NY, USA, 174–183. https://doi.org/10.1145/3578503.3583621
