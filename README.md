# Heart Disease Prediction using Decision Trees and Random Forests

## Objective
To build tree-based models for classifying the presence of heart disease using patient data. The models used are:
- **Decision Tree Classifier**
- **Random Forest Classifier**

## Tools Used
- Python
- Scikit-learn
- Pandas
- Graphviz
- Matplotlib (optional for visualization)

## Dataset Features
The dataset includes the following features:

| Feature | Description |
|---------|-------------|
| age | Age of the patient |
| sex | Gender (1 = male; 0 = female) |
| cp | Chest pain type (0-3) |
| trestbps | Resting blood pressure |
| chol | Serum cholesterol (mg/dl) |
| fbs | Fasting blood sugar > 120 mg/dl (1 = true; 0 = false) |
| restecg | Resting ECG results (0-2) |
| thalach | Maximum heart rate achieved |
| exang | Exercise-induced angina (1 = yes; 0 = no) |
| oldpeak | ST depression induced by exercise |
| slope | Slope of the peak exercise ST segment |
| ca | Number of major vessels (0-3) colored by fluoroscopy |
| thal | Thalassemia (0 = normal; 1 = fixed defect; 2 = reversible defect) |
| target | Presence of heart disease (1 = yes; 0 = no) |

## Workflow
1. **Data Preprocessing**
   - Handle missing values
   - Encode categorical variables

2. **Model Building**
   - Train a Decision Tree Classifier
   - Train a Random Forest Classifier

3. **Evaluation**
   - Accuracy Score
   - Confusion Matrix
   - Classification Report

4. **Visualization**
   - Visualize the Decision Tree using Graphviz

## Results
- Accuracy and performance metrics are printed for both models.
- The Decision Tree is visualized using Graphviz for better interpretability.

## Installation

Install the required libraries:

```bash
pip install pandas scikit-learn graphviz matplotlib
```
## What We Did

1. **Loaded and Explored the Dataset**  
   - Loaded a heart disease dataset containing 14 medical attributes per patient.
   - Checked for missing values and understood feature distributions.

2. **Preprocessed the Data**  
   - Converted appropriate columns to categorical types.
   - Separated the features (`X`) and target (`y`).
   - Split the dataset into training and testing sets using an 80-20 ratio.

3. **Trained a Decision Tree Classifier**  
   - Built a simple interpretable model using `DecisionTreeClassifier` from Scikit-learn.
   - Tuned `max_depth` to avoid overfitting.
   - Evaluated the model with accuracy, classification report, and confusion matrix.

4. **Visualized the Decision Tree**  
   - Used `Graphviz` to generate and render a visual representation of the decision tree.
   - This helped us interpret the decision-making process of the model.

5. **Trained a Random Forest Classifier**  
   - Built a more robust ensemble model using `RandomForestClassifier`.
   - Compared its accuracy and performance with the Decision Tree.

6. **Evaluated Both Models**  
   - Measured accuracy and analyzed predictions on test data.
   - Compared Decision Tree and Random Forest results to determine which performed better.
