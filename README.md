# Falcon 9 First Stage Landing Prediction

This project aims to predict the success of Falcon 9’s first stage landing using machine learning models. The project uses historical data from SpaceX launches to create predictive models that help assess the likelihood of a successful landing. By understanding the factors that contribute to landing success, we can better evaluate the cost-efficiency and technological advancements made by SpaceX.

---

## Project Overview

SpaceX has revolutionized the aerospace industry with its **Falcon 9** rocket, the first orbital-class rocket capable of reflight. Unlike traditional rockets that are discarded after use, the Falcon 9’s first stage is designed to return and land safely for reuse, greatly reducing the cost of space missions.

The goal of this project is to predict whether the Falcon 9's first stage will successfully land. This is achieved by analyzing a dataset of past SpaceX launches and applying machine learning models to predict landing outcomes based on various factors such as payload mass, launch site, weather conditions, and more.

---

## Dataset Overview

The dataset contains detailed information from previous SpaceX launches, including:

- **Flight Number**: A unique identifier for each mission.
- **Launch Site**: The location from which the rocket was launched, which can influence landing success based on weather conditions and proximity to landing zones.
- **Payload Mass (kg)**: The weight of the payload. Heavier payloads might affect the rocket’s fuel usage and landing performance.
- **Booster Version**: The specific version of the Falcon 9 used. Different booster versions may have different success rates due to improvements in design and technology.
- **Orbit Type**: The type of orbit for which the payload is intended (e.g., Low Earth Orbit, Geostationary Orbit). This can influence how much fuel is required and the feasibility of a return landing.
- **Weather Data**: Atmospheric conditions during the launch. Strong winds or poor weather could negatively impact the rocket's ability to land safely.
- **Landing Outcome**: The target variable, indicating whether the Falcon 9 first stage successfully landed (1) or failed (0).

---

## Why Reusable Rockets Matter

### About Falcon 9

The **Falcon 9** is a partially reusable two-stage rocket developed by SpaceX. Since its first launch in **2010**, Falcon 9 has become one of the most frequently launched rockets in history, used for missions ranging from launching satellites to resupply missions for the International Space Station (ISS).

The Falcon 9’s first stage is equipped with landing legs and grid fins that allow it to return to Earth after delivering its payload into orbit. This stage can either land on a drone ship at sea or on land, depending on the mission profile.

### Benefits of Reusable Rockets

Reusable rockets offer significant advantages over expendable rockets, transforming the economics of space travel:

1. **Cost Savings**: Traditionally, the first stage of a rocket, which includes the engines and fuel tanks, represents a large portion of the overall cost. Reusing this component drastically lowers the cost per launch, making space travel more affordable.
   
2. **Increased Launch Frequency**: With the ability to reuse rockets, the turnaround time between missions is reduced. SpaceX has demonstrated the ability to launch, recover, refurbish, and re-launch a Falcon 9 rocket in a matter of weeks or even days, making space missions more frequent and responsive.

3. **Environmental Sustainability**: Reducing waste by recovering and reusing rockets contributes to a more sustainable approach to space exploration, minimizing the need to build new rockets for each mission.

4. **Innovation and Development**: The push for reusability has led to advancements in rocket design, materials, and landing techniques. SpaceX’s success with the Falcon 9 has laid the groundwork for even more ambitious projects, like **Starship**, which is designed to be fully reusable and capable of interplanetary travel.

---

## Machine Learning Models

In this project, three machine learning models were developed and evaluated to predict the landing outcome of the Falcon 9’s first stage:

1. **Logistic Regression**:
   - A popular model for binary classification problems.
   - It estimates the probability of a binary outcome (landing success or failure) using a logistic function.
   - It is simple and interpretable but can have limitations with non-linear relationships.

2. **Support Vector Machine (SVM)**:
   - A powerful algorithm used for classification tasks.
   - It works by finding the optimal hyperplane that separates the classes (successful vs. unsuccessful landings).
   - SVMs are robust and effective when dealing with high-dimensional spaces.

3. **Decision Tree**:
   - A non-linear algorithm that splits the data into subsets based on feature values.
   - It is easy to visualize and interpret but can be prone to overfitting.
   - Decision trees are useful for capturing complex relationships between variables.

Each model was fine-tuned using **GridSearchCV**, which allowed for the optimization of hyperparameters to improve model performance.

### Model Performance

- **Best Cross-Validation Accuracy**: After performing hyperparameter tuning, the models achieved a best cross-validation accuracy of **84.28%**.
- **Test Accuracy**: All models performed similarly on the test data, with an accuracy of **83.33%**.
  
The consistent performance across different models indicates that the features used in this dataset are effective in predicting the outcome of a Falcon 9 first stage landing.

---

## Project Workflow

1. **Data Preprocessing**: 
   - The data was cleaned, missing values were handled, and categorical features (such as launch site, booster version, and orbit) were encoded into numerical values for use in the machine learning models.

2. **Exploratory Data Analysis (EDA)**:
   - EDA was performed to identify trends and patterns in the data. Visualizations were created using **Matplotlib** and **Seaborn** to better understand the relationships between features and the landing outcome.

3. **Feature Engineering**: 
   - New features were created to capture important aspects of the data. For instance, the payload mass and orbit type were combined to assess how they jointly affect the landing outcome.

4. **Modeling**: 
   - The dataset was split into training and testing sets. Multiple models were trained and evaluated using accuracy, precision, recall, and F1 score to select the best-performing model.

5. **Hyperparameter Tuning**: 
   - GridSearchCV was used to fine-tune the hyperparameters of each model, improving their accuracy on the test set.

---

## How to Use This Repository

1. **Clone the repository**:
   ```bash
   git clone https://github.com/<your-username>/falcon9-landing-prediction.git
   cd falcon9-landing-prediction
