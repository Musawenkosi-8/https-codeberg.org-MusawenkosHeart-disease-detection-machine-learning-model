# Heart-disease-detection-machine-learning-model

❤️ Problem Definition

Objective:
To build a machine learning model that can predict the presence of heart disease in a patient based on clinical parameters.

Real-world context:
Heart disease is one of the leading causes of death worldwide. Early prediction and diagnosis using machine learning can assist healthcare professionals in making informed decisions, potentially saving lives. The model is trained on clinical attributes to determine whether a patient is likely to have heart disease.

Target variable:

    target (or goal):

        0 = No heart disease

        1–4 = Presence of heart disease

    Most studies, including this one, reframe this as a binary classification problem:

        0 → no disease

        1 → disease present (any of 1, 2, 3, or 4)

🔍 Processes Followed

    Data Understanding & Preprocessing

        Source: Cleveland Heart Disease dataset (UCI Repository)

        Selected 14 features out of the full 76 available.

        Checked for:

            Missing values

            Data types

            Class balance in target variable
    Exploratory Data Analysis (EDA)

        Correlation matrix and heatmap to find relationships between features

        Visualized feature distributions (e.g., age, sex, cholesterol)

        Plotted bar charts and boxplots comparing features across heart disease classes
    Feature Engineering

        Normalization/standardization of continuous features

        Encoding categorical variables (e.g., chest pain type, fasting blood sugar)

        Checked multicollinearity among variables
    Modeling

        Algorithms used:

            Logistic Regression

            Random Forest

            Support Vector Machine (SVM)

            K-Nearest Neighbors (KNN)

            XGBoost

        Data split:

            Train/test split (commonly 80/20)

        Evaluation metrics:

            Accuracy

            Precision, Recall, F1 Score

            Confusion Matrix

            ROC-AUC Curve
    Model Selection and Tuning

        Hyperparameter tuning via Grid Search or Random Search

        Cross-validation to avoid overfitting

        Feature importance plotted for tree-based models
    Model Interpretation

        Analyzed which features had the most impact (e.g., chest pain, max heart rate)

        Used SHAP values or built-in model interpretability (e.g., .feature_importances_)

✅ Outcome

    Best-performing model achieved high accuracy and recall, making it suitable for medical applications where minimizing false negatives is critical.

    Identified top predictive features like:

        Chest pain type

        Exercise-induced angina

        Maximum heart rate achieved

        ST depression (oldpeak)

    The model could be deployed in a clinical decision support tool to flag high-risk patients.

    Reproducible notebook created in Jupyter, with clean visualization and interpretation steps.
