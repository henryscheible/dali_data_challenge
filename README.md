# dali_data_challenge
Completed as part of the 23W application for the DALI Data Team.
## Part 1
My submission for Part 1 is stored in `analysis.ipynb` and starts with an exploration of each column of the dataset, as well as checking the correlations between columns.
This section is not designed to be presentatable, it is simply to help me understand the data and find patterns that could be interesting. I also use this section to help me find whether each column has significant outliers, which helps me reject them in later analyses.

The Highlights section contains my presentable visualizations

Finally, I export a csv file to use later for modeling

## Part 2
### Category Prediction Model
`transformers.ipynb` contains a finetuned BERT transformer model which takes the Product Name as an input and predicts which category the product belongs to

### Profit Prediction Model
`model.ipynb` contains a gradient boosted trees model which predicts profit. I used InterpretML's Explainable Boosting Machine which operates purely additively with respect to input features, allowing the model to be completely explainable. This allows feature and interaction importances to be ranked both globally (for the whole dataset), and locally (for an individual example).
