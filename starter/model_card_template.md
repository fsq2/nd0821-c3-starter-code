# Model Card

For additional information see the Model Card paper: https://arxiv.org/pdf/1810.03993.pdf

## Model Details
`RandomForestClassfire` using `scikit-learn` libary 
used for classfication problem. hyperparamet are on default
## Intended Use
The model is used for classifying employees' salary into <=50K and >50K, based on employees's information.
## Training Data
The data utilized for training this model came from the Census Beurau, and consists of salary information - More information here: https://archive.ics.uci.edu/ml/datasets/census+income
## Evaluation Data
Evaluation data comes from the same dataset, but it's from a 20% split of the samples not used during training.
## Metrics
```python
precision: 0.7269914926527455
recall: 0.6151832460732984
fbeta: 0.6664303438496988
```
## Ethical Considerations
The misuse of these census information can cause consequences to the lives of people surveyed and (possibly) other people in some related populations
## Caveats and Recommendations
The model was trained on data of people mostly from the USA. Hence it is not recommended to use the model to predict the salary type for people from other regions in the world, which might have very different feature distributions
