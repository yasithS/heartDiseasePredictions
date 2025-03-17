# Heart Disease Prediction

A machine learning model that predicts the presence of heart disease in patients based on clinical parameters.

## Overview

This project uses logistic regression to predict whether a patient has heart disease based on various medical attributes. The model achieves approximately 85% accuracy on training data and 82% accuracy on test data.

## Dataset

The dataset contains medical records of 303 patients with 14 attributes:

- **age**: Age in years
- **sex**: Gender (1 = male, 0 = female)
- **cp**: Chest pain type (0-3)
- **trestbps**: Resting blood pressure in mm Hg
- **chol**: Serum cholesterol in mg/dl
- **fbs**: Fasting blood sugar > 120 mg/dl (1 = true, 0 = false)
- **restecg**: Resting electrocardiographic results (0-2)
- **thalach**: Maximum heart rate achieved
- **exang**: Exercise induced angina (1 = yes, 0 = no)
- **oldpeak**: ST depression induced by exercise relative to rest
- **slope**: Slope of the peak exercise ST segment (0-2)
- **ca**: Number of major vessels colored by fluoroscopy (0-4)
- **thal**: Thalassemia (0-3)
- **target**: Heart disease diagnosis (1 = disease present, 0 = healthy)

## Model

The project uses scikit-learn's Logistic Regression model. The dataset is split into training (80%) and testing (20%) sets.

## Performance

- Training accuracy: 85.1%
- Testing accuracy: 81.9%

## Requirements

- Python 3.x
- NumPy
- Pandas
- scikit-learn

## Usage

1. Clone the repository:
   ```
   git clone https://github.com/yourusername/heartDiseasePredictions.git
   cd heartDiseasePredictions
   ```

2. Install required packages:
   ```
   pip install numpy pandas scikit-learn
   ```

3. Run the Jupyter notebook:
   ```
   jupyter notebook "Heart Disease Prediction.ipynb"
   ```

4. To use the prediction model with new data:

```python
# Example of how to use the prediction function
input_data = [41, 0, 1, 130, 204, 0, 0, 172, 0, 1.4, 2, 0, 2]
makePredictions(input_data)
```

## Example Input Explanation

The input parameters should be provided in the following order:

1. Age: 41 years
2. Sex: 0 (female)
3. Chest pain type: 1 (typical angina)
4. Resting blood pressure: 130 mm Hg
5. Serum cholesterol: 204 mg/dl
6. Fasting blood sugar: 0 (≤ 120 mg/dl)
7. Resting ECG: 0 (normal)
8. Maximum heart rate: 172 bpm
9. Exercise-induced angina: 0 (no)
10. ST depression: 1.4 mm
11. ST segment slope: 2 (upsloping)
12. Number of major vessels: 0
13. Thalassemia: 2 (normal)

## Author

Yasith Gunawardhana

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
 
