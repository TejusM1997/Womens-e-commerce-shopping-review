# Womens-e-commerce-shopping-review
This is a nlp project for text feature extraction and sentiments analysis

### Objective

The aim of this project is to extract text features from the reviews written by customers pertaining to the clothing items they had purchased from an e-commerce portal.
Using these extracted features or sentiments we have to predict if the customer is likely to recommend the item or not

### Methodology

1.  Exploratory data analysis was done to find out the mean length of reviews,word counts, popular categories, Part of speech tags etc.
2.  Then for predictive modelling  probabilistic machine learning model Multinomial Navie Bayes was used to predict th output classes (Recommended or Not Recommended) after text vectorization
3.  We know that LSTMs are well suited for tasks like sentiments analysis in the light of their ability to remember and update the contexts of the model as they go through the text information, which is why we used LSTMs as well
4.  Along with LSTM layers we also added to the Keras Sequential model SpatialDropout1D regularization layer because If adjacent frames within feature maps are strongly correlated  then regular dropout will not regularize the activations and will otherwise just result in an effective learning rate decrease. In this case, SpatialDropout1D will help promote independence between feature maps and should be used instead.
