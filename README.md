The performance of individual base models was not satisfactory:

KNN had moderate performance but could be improved.
CART and SVR struggled to capture the relationships in the data well.
No single model provided an optimal solution on its own.
Stacking was used to leverage the strengths of each base model and create a more powerful ensemble. The idea behind stacking is that by combining multiple weak models, we can reduce their individual weaknesses and create a better final prediction.

In this case, the StackingRegressor used the combined knowledge from KNN, DecisionTree, and SVR models, and then the meta-model (LinearRegression) learned how to combine their predictions effectively. 
This approach improved the overall accuracy and reduced the error, as evident from the best NMAE score of -40.60.
