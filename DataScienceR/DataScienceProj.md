# Your first data science project

## The Goal
Utilize your knowledge of R to do an analysis of a dataset, and employ some machine learning concepts to model a feature of the dataset. This is an example of doing *supervised machine learning* because we have labeled data with our answers, and we are trying to figure out a model to explain how the inputs can be used to come up with the output. Additional supporting material for machine learning concepts can be found in the DataScienceResources.md file.

### The dataset
Good potential data sources:
* [House price prediction, a regression example](https://www.kaggle.com/harlfoxem/housesalesprediction)
* [Predicting if a mushroom is poisonous, a classification example](https://www.kaggle.com/uciml/mushroom-classification)

Plenty of other sources too if you want to get creative, but these are pretty straightforward in terms of what your target is. If you find one that you're interested in doing, just make sure you have one parameter that is clearly the output. For now, we want to stay away from image recognition and natural language processing-type problems.

### How to do the project
* Start by doing an exploratory data analysis.
  * Investigate your data. What kind of distributions are inherent in your data? Are there outliers, missing or nonsensical values? If so, how are you going to deal with these? Do any parameters seem to be highly correlated to each other? Do we need to think about reducing the number of variables we are looking at? There's a lot of questions to ask here, but these may become more obvious as you work with the data.
  * Make use of visualizations! They can help a lot in understanding your data.
  * Helpful libraries: `dplyr` and `ggplot2` (please find a use to demonstrate your knowledge of both of these!)
  * __Deliverable__: Create a well-commented R Script that shows all the things you did for your exploratory data analysis, and why you did them. Use the `dyplr` and `ggplot2` libraries, along with any others you may find useful.
* Next, create a script that will take your original data and preprocess it.
  * These should be things you discovered during your initial data exploration. Do data need to be scaled? Do some variables need to be treated as categorical instead of numerical? Do you need to "bin" some continuous variables (i.e. turning a continuous variable into a category for 1-5, 6-10, etc...)? There are lots of things that may make sense to do.
  * __Deliverable__: Create a well-commented R Script that takes your original data and processes it into a way that has useful features to model your output variable.
* Finally, do some machine learning!
  * Now that you have a nice preprocessed data frame, test out a few different machine learning algorithms and see how well you can model your target variable!
  * Separate your data into training and testing sets.
  * Test out at least 3 different types of machine learning algorithms. Do some hyperparameter tuning to find optimal settings. For now, stay away from more complex neural networks (no CNN or RNN. Standard NN with less than 10 layers is OK, if you can explain with comments how it works)
    * Suggestions (some may be applicable only for classification or regression- read up!): random forest, decision tree, cubist, linear regression, Naive Bayes, knn, SVM
  * Which one performed the best? What measure did you use to evaluate that (there are multiple!)? Does there appear to be overfitting? How might overfitting change which algorithm you choose?
  * Helpful libraries: `caret`
  * __Deliverable__: An R script that tests out at least 3 machine learning algorithms with hyperparameter tuning and uses the `caret` library.
  * __Deliverable__: Some sort of text document (Markdown preferred, but Word doc, txt file, pdf are all fine) explaining why you chose the ML algorithms that you did, broadly how they work, what your results were, how much you should be able to trust your results. Include visuals for things like AUC curve, fitting y vs y_predicted, etc... to help your explanation.
