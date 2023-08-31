# Obesity Level Prediction Using Machine Learning

## Overview

Obesity is a global health crisis that affects millions of people. The complexity of predicting obesity levels stems from the myriad of contributing factors, ranging from quantitative metrics like weight and height to lifestyle habits like diet and physical activity. In this project, I focus on predicting an individual's obesity level based on these multifaceted features. 

My approach involves two main phases: feature selection and model training. I've implemented two types of feature selection methods, providing a comprehensive evaluation of how each feature contributes to the prediction. The models are trained on both selected features and all available features, giving insights into how feature selection impacts the performance of the predictive models. Algorithms used include Linear Regression, Random Forest, k-Nearest Neighbors, and Support Vector Machines, among others. Each model undergoes rigorous evaluation to gauge its effectiveness in predicting obesity levels.

One of the standout aspects of this project is its potential as a self-help pre-screening tool. All the selected features, such as Gender, Age, Weight, Height, and lifestyle choices like Frequency of Consuming High-Caloric Food (FCVC), are data points that individuals usually know about themselves. Therefore, anyone can use this tool to get an early indication of their obesity level, enabling them to take timely action.

The codebase is modular, well-documented, and adheres to best practices, making it easily adaptable for future improvements. I invite you to explore this repository and look forward to your contributions in making this an even more robust solution.


## Features in the Dataset

- Gender {Female,Male}
- Age numeric
- Height numeric
- Weight numeric
- family_history_with_overweight {yes,no}
- FAVC {yes,no}
- FCVC numeric
- NCP numeric
- CAEC {no,Sometimes,Frequently,Always}
- SMOKE {yes,no}
- CH2O numeric
- SCC {yes,no}
- FAF numeric
- TUE numeric
- CALC {no,Sometimes,Frequently,Always}
- MTRANS {Automobile,Motorbike,Bike,Public_Transportation,Walking}
- NObeyesdad {Insufficient_Weight,Normal_Weight,Overweight_Level_I,Overweight_Level_II,Obesity_Type_I,Obesity_Type_II,Obesity_Type_III}

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Models Used](#models-used)
- [Results](#results)
- [Contributing](#contributing)


## Installation

Dependencies include:
- pandas
- numpy
- sklearn
- matplotlib
- seaborn

## Usage

1. **Data Preprocessing:**

    First, preprocess your dataset by scaling or encoding as per the requirements.

    \```python
    from sklearn.preprocessing import StandardScaler
    ...
    \```

2. **Feature Selection:**

    Feature selection is done using Extra Trees Classifier.

    \```python
    from sklearn.ensemble import ExtraTreesClassifier
    ...
    \```

3. **Model Training:**

    Several models are trained including:
    - Linear Regression
    - Random Forest Classifier
    - k-Nearest Neighbors
    - Support Vector Machine (SVM)
    
    \```python
    from sklearn.linear_model import LinearRegression
    ...
    \```

4. **Evaluation:**

    Evaluate the model using metrics such as Mean Squared Error, Mean Absolute Error, and R-squared value.

    \```python
    from sklearn.metrics import mean_squared_error, mean_absolute_error, r2_score
    ...
    \```

## Models Used
- **Linear Regression**: R-squared value of 0.94 with all features and 0.87 with selected features.
- **Random Forest Classifier**: Accuracy of 0.94 with all features and 0.87 with selected features.
- **k-Nearest Neighbors**: Accuracy of 0.9 with all features and 0.88 with selected features.
- **Support Vector Machines**: Accuracy of 0.87 with all features and 0.73 with selected features.

## Results
- Feature selection proved to be a valuable step, although performance with all features was generally better.
- Random Forest Classifier showed the highest accuracy among all models.

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.


---

Made with :heart: by Maham Khokhar

