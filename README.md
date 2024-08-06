# Predictive Modeling for Agriculture

## Overview

Sowing Success: How Machine Learning Helps Farmers Select the Best Crops

Measuring essential soil metrics such as nitrogen, phosphorous, potassium levels, and pH value is an important aspect of assessing soil condition. However, it can be an expensive and time-consuming process, which can cause farmers to prioritize which metrics to measure based on their budget constraints.

Farmers have various options when it comes to deciding which crop to plant each season. Their primary objective is to maximize the yield of their crops, taking into account different factors. One crucial factor that affects crop growth is the condition of the soil in the field, which can be assessed by measuring basic elements such as nitrogen and potassium levels. Each crop has an ideal soil condition that ensures optimal growth and maximum yield.

A farmer reached out to you as a machine learning expert for assistance in selecting the best crop for his field. They've provided you with a dataset called `soil_measures.csv`, which contains:

- `N`: Nitrogen content ratio in the soil
- `P`: Phosphorous content ratio in the soil
- `K`: Potassium content ratio in the soil
- `pH`: Value of the soil
- `crop`: Categorical values that contain various crops (target variable)

Each row in this dataset represents various measures of the soil in a particular field. Based on these measurements, the crop specified in the `crop` column is the optimal choice for that field.

In this project, you will apply machine learning to build a multi-class classification model to predict the type of `crop`, while using techniques to avoid multicollinearity, which is a concept where two or more features are highly correlated.

## Libraries Used

- `pandas`: For data manipulation and analysis.
- `numpy`: For numerical operations.
- `scikit-learn`: For building and evaluating the machine learning model.
- `matplotlib`: For data visualization.
- `seaborn`: For creating attractive and informative statistical graphics.

## Data

The dataset used is `soil_measures.csv` and includes the following columns:
- `N`: Nitrogen content ratio in the soil
- `P`: Phosphorous content ratio in the soil
- `K`: Potassium content ratio in the soil
- `pH`: Value of the soil
- `crop`: Target variable indicating the optimal crop for the field

## Analysis Steps

1. **Load and Inspect Data**: Load the dataset and inspect its structure and contents.
2. **Individual Feature Analysis**: Train logistic regression models for each soil metric and evaluate their performance.
3. **Correlation Analysis**: Calculate the correlation matrix and visualize it to identify multicollinearity.
4. **Feature Selection**: Choose a subset of features based on the analysis.
5. **Final Model Training and Evaluation**: Train a logistic regression model using the selected features and evaluate its performance.

## Insights

- **Individual Feature Performance**: Potassium (K) demonstrated the highest F1-score among individual features.
- **Correlation Analysis**: The correlation matrix indicated potential multicollinearity between features.
- **Final Model Performance**: A logistic regression model trained on the selected features (N, K, pH) achieved an improved F1-score of 0.5580.

## Conclusion

In this project, we addressed the challenge of assisting a farmer in crop selection based on soil metrics. The dataset provided information on nitrogen (N), phosphorous (P), potassium (K) levels, and pH value, along with the corresponding optimal crop for each field. We approached the problem using machine learning, specifically a logistic regression model.

The model demonstrated promise, showing improved performance with selected features. Future work could involve further refinement of the model to enhance accuracy in crop recommendations.

## Requirements

To run this project, you need the following Python libraries installed:

- `pandas`
- `numpy`
- `scikit-learn`
- `matplotlib`
- `seaborn`

## Usage

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/yourusername/predictive-modeling-agriculture.git
    ```
2. **Navigate into the Project Directory**:
    ```bash
    cd predictive-modeling-agriculture
    ```
3. **Install the Required Libraries**:
    ```bash
    pip install pandas numpy scikit-learn matplotlib seaborn
    ```
4. **Run the Jupyter Notebook**:
    Launch Jupyter Notebook and open the `predictive_modeling_agriculture.ipynb` file to start the analysis.
    ```bash
    jupyter notebook predictive_modeling_agriculture.ipynb
    ```
```

