# parkinson-disease-detection
Machine learning project for Parkinson's disease classification using voice measurements.
# Parkinson's Disease Detection Using Machine Learning

## Project Overview

This project explores the use of machine learning to distinguish between healthy individuals and people with Parkinson's disease based on voice measurements.

The objective is to investigate whether acoustic features can help identify vocal patterns associated with Parkinson's disease.

This is an educational machine learning project and is not intended for medical diagnosis.

## Dataset

The dataset is obtained from the **UCI Machine Learning Repository**.

It contains 195 voice recordings and 22 acoustic features, including:
- Jitter: variations in voice frequency.
- Shimmer: variations in voice amplitude.
- HNR: Harmonics-to-Noise Ratio.
- Other acoustic measurements.

The target variable is `status`:
- `0`: Healthy
- `1`: Parkinson's disease

## Methods and Tools

The project was developed using Python and the following libraries:

- **Pandas & NumPy** – Data manipulation and processing.
- **Matplotlib & Seaborn** – Data visualization.
- **Scikit-learn** – Machine learning and model evaluation.

The main steps include:

1. Exploratory Data Analysis (EDA)
2. Data preprocessing and feature scaling
3. Train/test split, keeping recordings from the same participant together
4. Training a Support Vector Machine (SVM) with a linear kernel
5. Model evaluation using accuracy, precision, recall, F1-score and a confusion matrix

## Results

The model achieved an accuracy of **78.4%** on the test set (29 correctly classified recordings out of 37).

The confusion matrix showed:
- 3 correctly classified healthy recordings.
- 26 correctly classified Parkinson's recordings.
- 8 misclassified recordings.

These results are preliminary and should be interpreted with caution due to the small test set and class imbalance.

## Project Structure

```text
parkinsons-disease-detection/
│
├── Parkinson_Detection_project.ipynb
├── parkinson.csv.txt
└── README.md
```

## How to Run

1. Clone this repository:
   ```bash
   git clone YOUR_REPOSITORY_URL
   ```
   
2. Install the required libraries:
   ```bash
   pip install numpy pandas matplotlib seaborn scikit-learn
   ```

3. Place the dataset file (`parkinson.csv.txt`) in the same directory as the notebook.

4. Open `Parkinson_Detection_project.ipynb` using Jupyter Notebook and run the cells.

## Future Improvements

- Test other machine learning algorithms.
- Explore feature selection techniques.
- Improve model evaluation using a larger dataset.
- Investigate methods to address class imbalance.

---

**Disclaimer:** This project is for educational purposes only and does not constitute a medical diagnostic tool.
