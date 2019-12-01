# Data Science
## Example Projects

Scroll down to see a preview of the contents: **[preview](#preview-of-example-projects)**

Here is a list of example projects for data science:

* [Visualization of the iris dataset](01_Visualization_Iris/Visualizition%20with%20pandas%20matplotlib%20seaborn.ipynb
  "Visualizition with pandas matplotlib seaborn.ipynb") - [preview](#visualization)
* [Prediction with Regression Models](02_Regression/Regression%20with%20sklearn.ipynb
"Regression with sklearn.ipynb") - [preview](#regression-models)
* [Prediction with Polynomial Models and Trees](02_Regression/Polynomial%20Regression%20and%20Trees.ipynb
"Polynomial Regression.ipynb") - [preview](#Polynomial-Models-and-Trees)
* [Scaling Pipelines Cross-Validation](02_Regression/Scaling%20Pipelines%20Cross-Validation.ipynb
"Scaling Pipelines Cross-Validation.ipynb") - [preview](#Scaling-Pipelines-Cross-Validation)

## Preview of example projects
### Visualization
**[notebook](01_Visualization_Iris/Visualizition%20with%20pandas%20matplotlib%20seaborn.ipynb
  "Visualizition with pandas matplotlib seaborn.ipynb")**

**pairplot**<br>
![pairplot](images/pairplot%20preview.jpg)<br><br>
**heatmap**<br>
![heatmap](images/heatmap%20preview.jpg)<br><br>
**violinplot**<br>
![violinplot](images/violinplot%20preview.jpg)<br><br>

### Regression Models
**[notebook](02_Regression/Regression%20with%20sklearn.ipynb
"Regression with sklearn.ipynb")**

**jointplot**<br>
![jointplot regression](images/regression%20jointplot.jpg)<br><br>
**OLS summary**<br>
![OLS summary](images/OLS%20summary.jpg)<br><br>
**Linear Regression, Runge, Lasso, Elastic Net Comparsion**<br>
![linear model](images/linear%20outliers.jpg)
![lasso model](images/lasso%20outliers.jpg)<br><br>

### Polynomial Models and Trees
**[notebook](02_Regression/Polynomial%20Regression.ipynb
"Polynomial Regression.ipynb")**

**Polynomial Features**<br>
![polynomial regression](images/polynomial%20regression.jpg)<br><br>
**Decision Tree Regression**<br>
![decision tree regression](images/regression%20tree.jpg)<br><br>
**Feature Importances**<br>
![Feature Importances](images/feature%20importance.jpg)<br><br>

### Scaling Pipelines Cross-Validation
**[notebook](02_Regression/Scaling%20Pipelines%20Cross-Validation.ipynb
"Scaling Pipelines Cross-Validation.ipynb")**

**StandardScaler, MinMaxScaler, MaxAbsScaler, Label Encoding**<br>

**One Hot Encoding**<br>
![One Hot Encoding](images/one%20hot%20heatmap.jpg)<br><br>

**Pipelines**
```python
from sklearn.pipeline import Pipeline
linear_pipeline = Pipeline([
    ('scaler', StandardScaler()),
    ('regressor', LinearRegression())
])
```

**Cross Validation**
```python
from sklearn.model_selection import cross_val_score

scores = cross_val_score(LinearRegression, X, y, cv=5)
print(scores)
```
