Classification
1. Standardization does not fix skewness.
2. Normalization does not handle outliers well since the outliers will be scaled down to between 0-1.
3. Normalization forces data to follow a Gaussian distribution. Standardization is usually used when the data is already following a Gaussian distribution, hence centering around the mean (0) with unit std dev (1).
4. Since we are using tree-based algorithms, standardization/normalization does not help much as these models are insensitive to the scale of the features.

--------------------------------------------------------------------------

1. It's fine to make assumptions and plot graphs feature by feature. To make things neater, plot graphs side by side or in the same figure to make clear comparisons.
2. When the number of features are manageable, plotting graphs feature by feature is still a good way. Otherwise, insights might be lost as we inspect more features.
3. When separating data into bins, make use of the quantile range, though manually assigning ranges is somewhat a quicker way.
4. When visualizing the performance of the models, make use of classification report and confusion matrix where the numbers tell a better story instead of just accuracy. Again, accuracy is not always the best metric for classification tasks.
5. If you have multiple models, make a table comparing the performances of each model for easy visualization.
6. Depending on the goal of the task, tweaking the threshold for classification is important. In this loan eligibility task, the threshold for loan approvals is usually lower than 0.5.