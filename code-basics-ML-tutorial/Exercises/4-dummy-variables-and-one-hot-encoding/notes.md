# Variables

## Types of Categorical Variable
- **Nominal**: No relation between variables
  > example ``` red, green, blue ```
- **Ordinal**: There is relation (ordering type of relation) between variables
  > example ``` high, medium, low ```

## Dummy Variables
Since categorical variable would not make any sense to regression algorithm, we can apply **'one hot encoding'** to these variable.
As a result of applying one hot encoding, for each categorical variable a column will be added and for the rows which belong to a specific category the category column would be set to one.
These new columns with '1' indicating the rows of category and rest rows set to '0' are called dummy variable.

**Example:** 


<img width="809" alt="image" src="https://github.com/VFulara/ML-basics/assets/56109892/d1b16a2c-4a1d-4351-8df7-4f40fda1c8dd">


## Dummy variable trap
Whenever there are correlated independent variables, these veriables can impact the accuracy of regression type of algorithms.
Introducing dummy variables for one hot encoding can cause this dummy variable trap and inorder to avoid it we can drop one of the dummy variable column
For more on dummy variable trap and collinearity [refer this](https://www.analyticsvidhya.com/blog/2020/03/what-is-multicollinearity/#:~:text=Multicollinearity%20is%20a%20statistical%20phenomenon,relationship%20among%20the%20predictor%20variables.)
