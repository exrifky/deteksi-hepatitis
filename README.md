# Hepatitis Detection 
**Problem**\
-Hepatitis infect many people in the world\
-This disease has relatively common symptoms so that it is prone to being underestimated by the public.
-Early detection is used to prevent the spread of hepatitis\

**Solution**\
-Using a machine learning approach to assist in the early detection of hepatitis\

**Dataset**\
-Taken  Kaggle data\
-Consists of 155 rows of data and 20 columns (features)\
-The distribution between classes is 32 lines for positive hepatitis.

**Methodology**\
-Research using the following methods (Fig. 1)\
-*random forest* as the main machine learning algorithm\
-*support vector machine - recursive feature elimination (SVM-RFE)* used for feature selection\
-*synthetic minority over-sampling technique* is used for *resampling dataset*\
-*grid search* is used for *hyper-parameter tuning*\
![alt text](https://i.ibb.co/5Kb44KK/Group-50.png)

**Result**\
-SVM_RFE results in the use of 7 features giving optimal results (Fig. 2)\
![alt text](https://i.ibb.co/Nj98bPQ/hasil-rfe.png)\
-*Resampling* using SMOTE results in a total dataset of 232, 116 for each class\
-*Hyper-parameter tuning* using GS produces the following *hyperparamter* values
| *hyper-parameters Tuning* | *Value*  |
| :---:   | :-: |
| *boostrap* | *false* |
| *max_depth* | 8  |
| *max_features* | 3 |
| *min_samples_leaf* | 2 |
| *min_samples_split* | 6  |
| *n_estimators* | 100 |

-The results of the *Random Forest Classifier* (RFC) are as follows
| *Accuracy* | *Precision*  | *ROC*  |
| :---: | :-: | :-: |
| 0.879 | 0.902 | 0.966 |

![alt text](https://i.ibb.co/cLRc8Q7/new.jpg)

**Limitation**\
Increasing the number of datasets and exploring hyperparameter optimization methods such as particle swarm optimization and genetic algorithms
