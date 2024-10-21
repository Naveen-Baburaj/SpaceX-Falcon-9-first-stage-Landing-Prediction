# SpaceX Falcon 9 First Stage Landing Prediction

This project aims to predict the successful landing of the first stage of SpaceX's Falcon 9 rockets. By analyzing key data points from previous launches, we explore different machine learning models to find the one that best predicts if the first stage of the rocket will land successfully, which is crucial for improving the cost-efficiency of space missions.

<div align="center">
    <img src="https://media2.giphy.com/media/v1.Y2lkPTc5MGI3NjExZzlla2JvbXAwNWJxOXc0ZGR4ajVjcmdobnNkMnlxeHgyN3cxMGt5NCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/xT39CRup15MdJgjLy0/giphy.webp" alt="SpaceX Falcon 9" />
</div>

## Project Overview

### Motivation

SpaceX revolutionized space travel by making the first stage of their Falcon 9 rocket reusable. Unlike traditional rockets, which are discarded after a single use, Falcon 9's first stage is designed to land safely back on Earth after launching its payload into space. This reusability drastically reduces launch costs, making space exploration more accessible and sustainable. Predicting whether the first stage will land successfully allows for further optimization of launches, helping ensure cost efficiency and improved planning.

<div align="center">
    <img src="https://www.stratfor.com/sites/default/files/styles/wv_small/public/asdf.png?itok=Zd0yuffv" alt="SpaceX Falcon 9" />
</div>

### Key Benefits of Reusable Rockets
- **Cost Reduction**: Traditional rockets are single-use, leading to high production costs for each launch. Reusable rockets allow for multiple uses of the same hardware, reducing the cost per launch significantly.
- **Sustainability**: By reusing rockets, fewer resources are needed, making the overall process more environmentally friendly.
- **Increased Launch Frequency**: With reduced costs, companies like SpaceX can increase the frequency of their launches, accelerating advancements in space exploration and technology.

### Machine Learning Approach

To predict the outcome of a Falcon 9 landing, the project uses the following process:
1. **Data Collection and Cleansing**: The dataset was collected from publicly available data on SpaceX launches. We processed and cleansed the data to remove inconsistencies and prepare it for analysis.
2. **Exploratory Data Analysis (EDA)**: EDA techniques were used to understand the relationships between different variables and their impact on the landing success of Falcon 9's first stage.
3. **Model Training**: Various machine learning models were trained and tested, including Logistic Regression, Decision Trees, and others. The models were tuned using GridSearchCV to find the best hyperparameters.

## Key Findings

- The best-performing models achieved an accuracy of **83.33%**, both during cross-validation and when tested on the holdout test set.
- Hyperparameter tuning using GridSearchCV yielded optimal parameters, with the best accuracy around **85%**.
- While the accuracy is encouraging, further optimization could be achieved by incorporating more advanced features and techniques.

## Files in This Repository

1. **[Collecting and Cleansing Data Notebook](https://github.com/Naveen-Baburaj/SpaceX-Falcon-9-first-stage-Landing-Prediction/blob/main/Collecting%20and%20Cleansing%20Data.ipynb)**: Detailed steps for collecting, cleansing, and preprocessing the SpaceX launch data.
2. **[Exploratory Data Analysis (EDA) Notebook](https://github.com/Naveen-Baburaj/SpaceX-Falcon-9-first-stage-Landing-Prediction/blob/main/Exploratory%20Data%20Analysis.ipynb)**: Visualizations and analysis of the key variables impacting the landing success.
3. **[Machine Learning Model Notebook](https://github.com/Naveen-Baburaj/SpaceX-Falcon-9-first-stage-Landing-Prediction/blob/main/Machine%20Learning.ipynb)**: Model training, hyperparameter tuning, and evaluation.
4. **[Dataset](https://github.com/Naveen-Baburaj/SpaceX-Falcon-9-first-stage-Landing-Prediction/blob/main/SpaceXdataset.csv)**: The dataset used for this project.

## Technologies Used
- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib & Seaborn** (for visualizations)
- **Scikit-Learn** (for machine learning models)

## Conclusion

This project highlights the potential of machine learning in predicting the success of SpaceX Falcon 9's reusable first stage. With an accuracy of over 83%, the models show promise in improving launch planning and efficiency. 

For further details, please explore the [full repository](https://github.com/Naveen-Baburaj/SpaceX-Falcon-9-first-stage-Landing-Prediction).
