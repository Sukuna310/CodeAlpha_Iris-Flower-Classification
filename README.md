# 🌸 Iris Flower Classification

A machine learning project that classifies Iris flowers into three species (Setosa, Versicolor, Virginica) based on their physical measurements using the K-Nearest Neighbors (KNN) algorithm.

## 📊 Dataset Overview

The famous Iris dataset, originally published by R.A. Fisher in 1936, contains 150 samples with 4 features:

| Feature | Description | Range |
|---------|-------------|-------|
| Sepal Length | Length of the sepal (cm) | 4.3 - 7.9 |
| Sepal Width | Width of the sepal (cm) | 2.0 - 4.4 |
| Petal Length | Length of the petal (cm) | 1.0 - 6.9 |
| Petal Width | Width of the petal (cm) | 0.1 - 2.5 |

**Classes:**
- Iris-Setosa (50 samples)
- Iris-Versicolour (50 samples)
- Iris-Virginica (50 samples)

## 🔬 Project Workflow

### 1. Data Loading & Exploration
- Load Iris dataset using scikit-learn
- Create pandas DataFrame with feature columns
- Examine data structure with `info()` and `describe()`
- Check class distribution (50 samples per class)

### 2. Data Visualization
- **Pairplot**: Visualize relationships between all features colored by species
- **Correlation Heatmap**: Show feature correlations (petal length/width show high correlation ~0.95)

### 3. Model Training
- Split data: 80% training (120 samples), 20% testing (30 samples)
- Train KNN classifier with k=3 neighbors
- Achieved **100% accuracy** on test set

### 4. Model Evaluation
- **Classification Report**: Precision, Recall, F1-Score for each class
- **Confusion Matrix**: Visual representation of predictions vs actual
- **Hyperparameter Tuning**: Test k values from 1 to 20 to find optimal neighbors

## 🎯 Results

| Metric | Score |
|--------|-------|
| Accuracy | 100% |
| Precision (per class) | 1.00 |
| Recall (per class) | 1.00 |
| F1-Score (per class) | 1.00 |

The model perfectly classifies all three Iris species, which is expected given the well-separated clusters in the Iris dataset.

## 🛠️ Tech Stack

- **Python**: Programming language
- **pandas**: Data manipulation
- **numpy**: Numerical computing
- **matplotlib**: Basic plotting
- **seaborn**: Statistical visualization
- **scikit-learn**: Machine learning library

## 📈 Key Learnings

1. **Supervised Classification**: Learning from labeled training data to predict labels for new data
2. **Train/Test Split**: Essential for evaluating model performance on unseen data
3. **KNN Algorithm**: Finds k nearest neighbors and votes on the class
4. **Precision vs Recall**: Understanding different evaluation metrics
5. **Confusion Matrix**: Visualizing where the model makes mistakes
6. **Hyperparameter Tuning**: Finding the optimal value of k for KNN

## 🚀 Why KNN for Iris?

- **Small, clean dataset**: KNN works well with moderate-sized datasets
- **Clear class separation**: The three species form distinct visual clusters
- **Interpretability**: Easy to explain — "find similar flowers and vote"
- **No training phase**: Model simply stores training data and computes distances at prediction time

## 📝 Usage

Open the Jupyter notebook to see the complete analysis:

```bash
jupyter notebook Iris_Classification.ipynb
```

Or run the code sections sequentially to:
1. Explore the data
2. Visualize relationships
3. Train the model
4. Evaluate performance
5. Tune hyperparameters

