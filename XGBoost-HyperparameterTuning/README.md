# XGBoost - Hyperparameter-Optimization

XGBoost Advantage:
1. Regularization - Standard GB has no regularization. Hence this helps in reducing overfitting.
2. Parallel Processing - Hence makes it faster
3. Handling Missing Values - 
4. Tree Pruning - GBM would stop splitting a node when it encounters a negative loss in the split. Thus it is more of a greedy algorithm.
                - It makes splits upto the max_depth specified and then start pruning the tree backwards and remove splits beyond which there is no positive gain.
5. Built-in CrossValidation - Allows user to run a cross-validation at each iteration.

---------------------------------------------------------------------------------------------------

XGBoost Parameters:

1. General Parameters: 
    - booster (default=gbtree)
    - silent  (default = 0)
    - nthread (defaut to maximum number of threads)

2. Booster Parameters:
    - eta
    - min_child_weight (default=1): Defines the minimum sum of weights of all observations
    - max_depth (default=6): Used to control over-fitting
    - max_leaf_nodes: maximum number of terminal nodes or leaves in a tree
    - gamma: A node is split only when the resulting split gives a positive reduction in the loss function. Gamma specifies the minimum loss reduction required to make a split.
    - max_delta_step:
    - subsample:
    - colsample_bytree:
    - colsample_bylevel:
    - lambda:
    - alpha:
    - scale_pos_weight:

3. Learning Task Parameters:
    - objective (default=reg:linear)
    - eval_metric (default according to objective)
    - seed(default:0)



https://github.com/dmlc/xgboost/tree/master/demo/guide-python
https://www.analyticsvidhya.com/blog/2016/03/complete-guide-parameter-tuning-xgboost-with-codes-python/
https://towardsdatascience.com/doing-xgboost-hyper-parameter-tuning-the-smart-way-part-1-of-2-f6d255a45dde
