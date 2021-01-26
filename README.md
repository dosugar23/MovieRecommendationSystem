# Movie Recommendation System
MovieLens-Recommender is a University project of Artificial Intelligence course. Implement of Collaborative Filtering. Which contains User Based Collaborative Filtering and Item Based Collaborative Filtering.
The buildin-datasets are Movielens-1M and Movielens-100k

# Overview
My Recommendation System contains four steps:

- Create trainset and testset
- Train a recommender model
- Give recommendations
- Evaluate results

At the end of a recommendation process, four numbers are given to measure the recommendation model, which are:

- Precision
- Recall
- Coverage
- Popularity
**No python extensions(e.g. Numpy/pandas) are needed!**
# How to run project
The configures are in `main.py`. Pleas choose the dataset and model you want to use and set the proper test_size. The default values in `main.py` are shown below:

```python
dataset_name = 'ml-100k'
# dataset_name = 'ml-1m'
# model_type = 'UserCF'
model_type = 'ItemCF'
test_size = 0.1
```

Then run ``python main.py`` in your command line. There will be a recommendation model built on the dataset you choose above.

Note: my code only tested on python3, so python3 is prefer.

This command will run in background. You can wait for the result, or use `tail -f run.log` to see the real time result.

All model will be saved to `model/` fold, which means the time will be cut down in your next run.
