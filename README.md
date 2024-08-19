# Speech Emotion Recognition

This project focuses on implementing Speech Emotion Recognition using the Torrento Dataset. The model is built using a combination of Convolutional Neural Network (CNN) and Long Short-Term Memory (LSTM) recurrent neural network.

## Dataset

The Torrento Dataset consists of audio recordings labeled with seven different emotion classes: happy, sad, angry, fear, disgust, neutral, and surprise. The dataset provides a diverse range of emotions for training and evaluation.

## Model Architecture

The model architecture combines the power of CNN and LSTM to capture both local and temporal features from the audio data. The CNN layers extract high-level features from the spectrogram representation of the audio, while the LSTM layers capture the temporal dependencies in the sequence of frames.

## Usage

To use this project, follow these steps:

1. Download the Torrento Dataset and preprocess the audio files.
2. Split the dataset into training, validation, and testing sets.
3. Train the CNN-LSTM model using the training set.
4. Evaluate the model's performance on the validation set.
5. Test the model on the testing set and analyze the results.

## Results

The performance of the model can be evaluated using metrics such as accuracy, precision, recall, and F1-score. The results will provide insights into the model's ability to recognize different emotions from speech.

## Conclusion

Speech Emotion Recognition is an important task in various applications, including human-computer interaction and sentiment analysis. This project demonstrates the effectiveness of the CNN-LSTM model in accurately classifying emotions from speech.
