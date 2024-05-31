# Heart Disease Classification

This project aims to classify whether a patient has heart disease or not using machine learning techniques. It utilizes a variety of features from medical examinations to make the prediction.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Model](#model)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Heart disease is a major health issue worldwide, and early detection is crucial for effective treatment. This project focuses on building a predictive model to classify the presence of heart disease based on several medical attributes. The goal is to help in early diagnosis and potentially save lives by enabling timely medical intervention.

## Dataset

The dataset used in this project is the [UCI Heart Disease Dataset](https://archive.ics.uci.edu/ml/datasets/Heart+Disease). It includes 303 instances with 14 attributes:

1. Age
2. Sex
3. Chest Pain Type (4 values)
4. Resting Blood Pressure
5. Serum Cholesterol in mg/dl
6. Fasting Blood Sugar > 120 mg/dl
7. Resting Electrocardiographic Results (values 0, 1, 2)
8. Maximum Heart Rate Achieved
9. Exercise Induced Angina
10. ST Depression Induced by Exercise Relative to Rest
11. Slope of the Peak Exercise ST Segment
12. Number of Major Vessels (0-3) Colored by Flourosopy
13. Thal (3 = normal; 6 = fixed defect; 7 = reversable defect)
14. Target (1 = presence of heart disease, 0 = absence)

## Installation

To get started with this project, follow these steps:

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/heart-disease-classification.git
    cd heart-disease-classification
    ```

2. Create and activate a virtual environment:
    ```sh
    python3 -m venv venv
    source venv/bin/activate   # On Windows use `venv\Scripts\activate`
    ```

3. Install the required dependencies:
    ```sh
    pip install -r requirements.txt
    ```

## Usage

To train the model and make predictions, follow these steps:

1. **Preprocess the data:**
    ```sh
    python preprocess.py
    ```

2. **Train the model:**
    ```sh
    python train.py
    ```

3. **Make predictions:**
    ```sh
    python predict.py --input data/input_data.csv
    ```

## Model

The project uses several machine learning algorithms to find the best performing model for heart disease classification. The main steps include:

1. **Data Preprocessing:** Handling missing values, encoding categorical features, and scaling numerical features.
2. **Model Training:** Using algorithms such as Logistic Regression, Random Forest, and Support Vector Machine (SVM).
3. **Evaluation:** Assessing the models using metrics like accuracy, precision, recall, and F1-score.

## Results

The results section will summarize the performance of the different models. For example:

- Logistic Regression: Accuracy - 85%
- Random Forest: Accuracy - 90%
- SVM: Accuracy - 88%

Detailed performance metrics and confusion matrices are available in the `results` directory.

## Contributing

Contributions are welcome! If you have any improvements or suggestions, please create a pull request or open an issue. For major changes, please discuss them in an issue first.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
