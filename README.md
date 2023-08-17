# Final-Project: Red or White?

### Team Members:

* Kelsey Richards
* Patrycja Pekala
* Nigan Marin
* Yanqiu Yang
* Jessica Ferraro

### Project Progress:

Using Python, machine learning, sklearn, pandas, and Tableau, our team is predicting wine type (red, white, other), price, and points and visualizing the data and results.

##### Steps:

1. Review & Preprocess Data:
   i. Clean data (looking out for null values, outliers)
   ii. Classify certain text columns as numeric / dummy encoding (one-hot-encoding the top 10 provinces of origin, for example)
2. Test several different machine learning models to predict price, points, and/or wine type based on the available information on each wine
   e.g. linear regression, PCA, multi-label classification, neural networks, etc.
   Which factors are driving the price? Which factors are driving points? How can we predict wine type?
3. Optimize models
4. Plot visualizations to summarize test and training data results, create visualizations of total dataset

##### Unsucessful Attempt:

At first, we wanted to do our project using a data set based on OkCupid dating profiles. This data set included information such as users age, sexual orientation, location, zodiac signs, and three essay prompts. Our intial idea was to use machine learning to see if we could predict zodiac signs of the users or if the users would be successful in getting a dating match. We tried many times to create a machine learning model, but the models were less than 20% accurate.

### Our Data Decription:

The data set we used for this project contains over 75k types of wine. The data list the location, designation, winery, desciprtion, review, and reviewers name. We added in a column for wine type. The wine type is red wine, white wine, or other. We used other to signify wines like Rose that could not be categorized as specifically red or white.

### Our Machine Learning Models:

We created a CatBoostRegressor model with 1000 iterations to predict the wine price. We created a neural network to predict wine type based on province of origin. It was based on the top 10 provinces that we one-hot-encoded. Our most successful model was predicting wine type using pycaret classification. We had several versions of this model. The first version predicted wine type using the text description from the data set. The second version of the model built on the first by adding province. The third version of the model included description, province, and designation. All three models yieled over 90% accuracy.

### Links to Data/Tableau Report/Presentation Slides:

* Link to dataset of wine: [click here to view](https://www.kaggle.com/code/pierreco/eda-worldwide-french-wines/input)
* Link to Tableau report of wine: [click here to view](https://public.tableau.com/app/profile/jessica.ferraro/viz/Wine_16917203318780/Top10?publish=yes)
* Link to Presentation Slides:[ click here to view](https://docs.google.com/presentation/d/1xKt4QAIv9kK5b7D9CmnzMaw93glQc4jb/edit#slide=id.g23bcb29e4ff_3_0)
