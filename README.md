# Explicit-negative-feedback-for-MF-models
Project on implementing negative feedback in the MF models

The implementation of the negative feedback (implicit and explicit) has bee proven to increase the performance metrics and the quality of the recommender systems. That's why the following project has a big importance and relevancy, as well as high potential for the future refining and improvements. The repository has 2 datasets with the explicit feedback (Amazon Toys & Games (https://cseweb.ucsd.edu/~jmcauley/datasets/amazon/links.html) and Movielens 1 M datatsets(https://grouplens.org/datasets/movielens/1m/)) and the main file with code (**CODE.ipynb**) with the code for all the proposed models and preprocessing techniques. 

In the course of work, 3 preprocesssing approaches as well as 3 models were implemented and tested.

The implemented preprocessing steps and strategies:
- filtering the dataset on the minimum number of interactions for each user (step)
- splitting the filtered data into 4 groups: training set, validation set, positive test set + positive holdout, negative test set + negative holdout (step)
- training the models on the full history (strategy)
- training the models on the positive history (strategy)
- training the models on the dual item embeddings (strategy)
- evaluating the model performance on the following metrics: pos_HR@10, neg_HR@10, diff_HR@10, pos_NDCG@10, neg_NDCG@10, diff_NDCG@10, MCC (step)

The models used in the experimental setting (implemented via implicit library):
- iALS (with hyperparameters tuning)
- BPR (with hyperparameters tuning)
- Popular recommendations

In order to conduct the experiments and test the results on your own you can use the mentined above code file (**CODE.ipynb**) with the desired changes (tune of the initial parameters of the split, hyperparameters of the model, number K of evaluations as in top_k and etc.)

Contributors of the project: Bogdan Monogov, Veronika Ivanova
