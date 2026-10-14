# SMS Spam Detection Using LSTM

## 1. Project Overview

SMS Spam Detection is a deep learning project that classifies text messages into two categories:

- **Spam:** Unwanted or potentially fraudulent messages.
- **Ham:** Normal and legitimate messages.

This project uses an LSTM (Long Short-Term Memory) neural network to learn patterns in SMS messages and predict whether a message is spam or normal.

## 2. Problem Statement

Mobile communication companies receive a large number of SMS messages every day. Identifying spam messages manually is difficult and time-consuming.

The objective of this project is to develop a deep learning model that automatically detects spam messages and helps improve message filtering.

## 3. Objectives

- Load and preprocess an SMS dataset.
- Convert text messages into numerical sequences.
- Build and train an LSTM deep learning model.
- Evaluate the model using accuracy, precision, recall, and F1-score.
- Display a confusion matrix.
- Predict whether new SMS messages are spam or normal.

## 4. Technologies Used

- **Programming Language:** Python
- **Platform:** Google Colab
- **Deep Learning:** TensorFlow and Keras
- **Data Processing:** Pandas and NumPy
- **Machine Learning Utilities:** Scikit-learn
- **Visualization:** Matplotlib and Seaborn

## 5. Dataset

**Dataset source:** [SMS Spam Detection Dataset on Kaggle](https://www.kaggle.com/datasets/vishakhdapat/sms-spam-detection-dataset)

The project uses approximately 2,000 labeled SMS messages.

The dataset contains message text and corresponding labels:

| Label | Meaning |
|---|---|
| Ham (0) | Normal message |
| Spam (1) | Spam message |

The dataset is cleaned by removing missing values and duplicate messages before training.

## 6. Project Workflow

1. Load the SMS dataset.
2. Clean the data and remove duplicates.
3. Separate messages and their labels.
4. Split the dataset into training and testing sets.
5. Tokenize messages into numerical sequences.
6. Apply padding to make sequences the same length.
7. Build the LSTM model.
8. Train the model using labeled messages.
9. Evaluate the model using performance metrics.
10. Predict spam or normal messages entered by the user.

## 7. Model Architecture

The project uses an LSTM neural network with the following layers:

1. **Embedding Layer:** Converts word indices into numerical vectors.
2. **LSTM Layer:** Learns sequential patterns and relationships between words.
3. **Dropout Layer:** Helps reduce overfitting during training.
4. **Dense Layer:** Learns patterns useful for classification.
5. **Output Layer:** Uses the sigmoid activation function to produce a spam score.

A score of 0.5 or higher is classified as spam; a lower score is classified as ham.

## 8. Installation and Execution

### Step 1: Open Google Colab

Visit [Google Colab](https://colab.research.google.com/) and create a new notebook.

### Step 2: Install the required libraries

```bash
pip install tensorflow pandas numpy scikit-learn matplotlib seaborn
```

### Step 3: Upload the dataset

Upload `spam_sms.csv` to the Google Colab environment.

### Step 4: Run the code

Copy the Python code into the notebook and execute the cells in order.

### Step 5: View the results

The notebook displays:
- Training and validation performance
- Accuracy, precision, recall, and F1-score
- Confusion matrix
- Predictions for new SMS messages

## 9. Evaluation Metrics

The model is evaluated using the following metrics:

- **Accuracy:** Measures the proportion of correctly classified messages.
- **Precision:** Measures how many predicted spam messages are actually spam.
- **Recall:** Measures how many actual spam messages are correctly detected.
- **F1-score:** Combines precision and recall into a single metric.
- **Confusion Matrix:** Shows correct and incorrect predictions for both classes.

Actual metric values should be added after running the model.

## 10. Sample Predictions

| SMS Message | Expected Classification |
|---|---|
| Congratulations! You won a free prize. Call now! | Spam |
| Hello, are you coming to college tomorrow? | Ham |
| URGENT! Claim your cash reward now! | Spam |
| Please send me the class notes. | Ham |

These are illustrative examples. Actual model predictions may differ.

## 11. Expected Outcome

The project demonstrates how deep learning can be applied to text classification. The trained model can classify unseen SMS messages and provide evaluation results to measure its performance.

The final performance depends on the dataset, preprocessing, training process, and model configuration.

## 12. Future Enhancements

- Compare LSTM with GRU and other classification models.
- Improve performance using a larger labeled dataset.
- Develop a web application for real-time SMS classification.
- Add message filtering and spam alerts.
- Evaluate the model on messages from different sources.

## 13. Conclusion

This project implements an SMS Spam Detection system using Python, TensorFlow, and LSTM. It demonstrates text preprocessing, tokenization, deep learning model training, performance evaluation, and prediction on new messages.

The project provides a foundation for developing automated spam detection systems for mobile communication.

## 14. Author

**Project:** SMS Spam Detection Using LSTM  
**Language:** Python  
**Platform:** Google Colab  
**Repository:** Add your GitHub repository URL here.
