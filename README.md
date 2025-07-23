# Optimizing-Energy-Efficiency

This project focuses on predicting office room occupancy using environmental factors like temperature, humidity, light, CO2 levels, and humidity ratio. The dataset, sourced from the UCI machine learning repository, contains minute-by-minute readings of these factors and the corresponding occupancy status.

Initial data analysis revealed no missing or duplicate values, but identified outliers and multicollinearity among features, particularly between humidity and humidity ratio, and notable correlations between light, CO2, and temperature.

Several classification models were implemented and evaluated, including Logistic Regression, K-Nearest Neighbors (KNN), Support Vector Classifier (SVC), Decision Tree Classifier, Random Forest, AdaBoost, Gradient Boosting, and XGBoost. Hyperparameter tuning using techniques like GridSearchCV was performed to optimize model performance.

The evaluation focused on accuracy and precision, with a baseline accuracy of approximately 79% on the test set. The results indicated that ensemble methods, particularly AdaBoost, achieved the highest accuracy (99.31%) and precision (97.37%) on the test data. Logistic Regression also performed well with high accuracy and fast training time.

The feature importance analysis from the Random Forest model highlighted Light, CO2, and Temperature as the most influential features. The AdaBoost model, interestingly, relied solely on the Light feature for its high performance, suggesting its significant predictive power in this context.

In conclusion, this project successfully demonstrates that accurate office room occupancy prediction is achievable using readily available environmental sensor data and various machine learning models. The AdaBoost model emerged as the best performer in terms of both accuracy and precision, making it a strong candidate for real-world applications in smart buildings and other environments where occupancy detection is crucial. The robustness of tree-based models to outliers was also observed.

### References

1.UCI Machine Learning Repository. (n.d.). Archive.ics.uci.edu. Retrieved July 21, 2023, from https://archive.ics.uci.edu/dataset/357/occupancy+detection

2.scikit-learn. (2019). scikit-learn: machine learning in Python. Scikit-Learn.org. https://scikit-learn.org/stable/

3.Horsch, A. (2021, December 21). Detecting And Treating Outliers In Python — Part 1. Medium. https://towardsdatascience.com/detecting-and-treating-outliers-in-python-part-1-4ece5098b755

‌4.Detecting Multicollinearity with VIF - Python. (2020, August 14). GeeksforGeeks. https://www.geeksforgeeks.org/detecting-multicollinearity-with-vif-python/

‌5.Candanedo,Luis. (2016). Occupancy Detection . UCI Machine Learning Repository. https://doi.org/10.24432/C5X01N.

6.Python API Reference — xgboost 1.5.0 documentation. (2021). Readthedocs.io. https://xgboost.readthedocs.io/en/stable/python/python_api.html

‌7.Feature importances with a forest of trees. (n.d.). Scikit-Learn. https://scikit-learn.org/stable/auto_examples/ensemble/plot_forest_importances.html
