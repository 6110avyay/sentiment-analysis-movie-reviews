# Sentiment Analysis of Movie Reviews Using Bidirectional LSTM

## Project Overview

This project uses a Bidirectional Long Short-Term Memory (BiLSTM) neural network to classify movie reviews as positive or negative.

The model is trained on the IMDb movie review dataset and evaluated on a separate test dataset. The project also explores sentiment predictions on a small collection of film reviews published by Decoders, A publication founded by Avyay Koppaka

## Objectives

- Build a neural network for movie review sentiment classification.
- Learn sentiment patterns from textual data using a Bidirectional LSTM.
- Evaluate the model using standard classification metrics.
- Explore the model's predictions on independent film reviews.

## Technologies Used

- Python
- TensorFlow and Keras
- NumPy and Pandas
- Scikit-learn
- Matplotlib
- Google Colab

## Methodology

1. Load the IMDb movie review dataset.
2. Preprocess and encode the review text.
3. Build a Bidirectional LSTM neural network.
4. Train the model using binary cross-entropy loss and the Adam optimizer.
5. Evaluate the model on the IMDb test dataset.
6. Generate a classification report and confusion matrix.
7. Apply the trained model to selected Decoders film reviews.

## Model Architecture

The neural network consists of:

- An embedding layer for word representations.
- A Bidirectional LSTM layer for sequential text processing.
- A dropout layer to help reduce overfitting.
- A dense output layer with sigmoid activation for binary classification.

## Results

The final model achieved the following results on the IMDb test dataset:

| Metric                  | Result |
| ----------------------- | -----: |
| Test accuracy           | 84.58% |
| Test loss               | 0.3701 |
| Negative-class F1-score |   0.85 |
| Positive-class F1-score |   0.84 |

The model was also tested on seven selected Decoders reviews. These predictions are exploratory and do not represent a formal accuracy evaluation on the Decoders collection.

## Limitations

- The model supports binary sentiment classification and does not explicitly identify mixed sentiment.
- The Decoders review collection is small and is not a representative evaluation dataset.
- Literary criticism may contain nuanced opinions that are difficult to classify using a binary sentiment model.
- The IMDb test results may not generalize directly to other sources of film reviews.

## Project Files

- `Sentiment_Analysis_LSTM.ipynb` – Notebook containing the implementation, training and evaluation.
- `decoders_sentiment_lstm.keras` – Saved trained model, if included in the repository.

## How to Run

1. Open the notebook in Google Colab.
2. Run the cells in order to reproduce the data preparation, training and evaluation.
3. Use the prediction function to classify new movie reviews.

## Conclusion

This project demonstrates the application of a Bidirectional LSTM neural network to sentiment analysis. It also explores the challenges of applying a model trained on IMDb reviews to independent film criticism.
