# Fake News Prediction Using AI/ML

## Overview

This project aims to predict whether a news article is real or fake using machine learning techniques in Python. The model is built with a focus on data pre-processing, feature extraction, and classification using logistic regression.

## Dataset

The dataset used for this project can be downloaded from Kaggle:

[Download train.csv](https://www.kaggle.com/c/fake-news/data?select=train.csv)

### About the Dataset

- **id**: Unique identifier for each news article
- **title**: Title of the news article
- **author**: Author of the article
- **text**: Content of the article (may be incomplete)
- **label**: Indicates whether the article is real (0) or fake (1)

## Dependencies

Make sure you have the following Python packages installed:

- numpy
- pandas
- nltk
- scikit-learn

You can install the required packages using pip:

```bash
pip install numpy pandas nltk scikit-learn
```

## Project Structure

The main code is contained in the `Fake News Prediction.ipynb` Jupyter notebook, which includes:

1. **Data Loading**: Loading the dataset into a pandas DataFrame.
2. **Data Pre-processing**: Handling missing values, merging text fields, and stemming the text.
3. **Feature Extraction**: Converting textual data to numerical data using TF-IDF Vectorization.
4. **Model Training**: Training a Logistic Regression model.
5. **Model Evaluation**: Evaluating the model's performance using accuracy metrics.
6. **Prediction**: Testing the model with new data.

## Getting Started

1. **Download the Dataset**: Ensure you have the `train.csv` file in your project directory.

2. **Run the Jupyter Notebook**: Open `Fake News Prediction.ipynb` and execute the cells sequentially.

3. **Model Training and Evaluation**: The notebook includes code to train the model and evaluate its accuracy on both training and test datasets.

## Example Usage

After running the model, you can test predictions using a sample from the test set:

```python
X_new = X_test[3]
prediction = model.predict(X_new)

if (prediction[0] == 0):
    print('The news is Real')
else:
    print('The news is Fake')
```

## Acknowledgments

- Dataset from [Kaggle](https://www.kaggle.com/c/fake-news/data?select=train.csv)
- NLTK library for natural language processing
- Scikit-learn for machine learning utilities

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Conclusion

This project serves as a foundational step in building AI/ML applications for text classification tasks. Happy coding!