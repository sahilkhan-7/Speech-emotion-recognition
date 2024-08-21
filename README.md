# 🎙️ Speech Emotion Recognition Using CNN-LSTM

## 👀 Overview 

This project aims to build a Speech Emotion Recognition (SER) model that can accurately classify emotions from speech data. Using a combination of Convolutional Neural Networks (CNN) and Long Short-Term Memory (LSTM) networks, the model is trained on the TESS, RAVDESS, SAVEE, and CREMA-D datasets. The goal is to classify six emotions: angry, happy, fear, sad, disgust, and neutral.

## 🗃️ Datasets

The datasets used in this project are:

- **TESS**: Toronto Emotional Speech Set
- **RAVDESS**: Ryerson Audio-Visual Database of Emotional Speech and Song
- **SAVEE**: Surrey Audio-Visual Expressed Emotion
- **CREMA-D**: Crowd-sourced Emotional Multimodal Actors Dataset

These datasets are combined and preprocessed to create a balanced and comprehensive dataset for emotion recognition.

## Features Extracted

Key audio features extracted using the `librosa` library include:

- **MFCC**: Mel-Frequency Cepstral Coefficients - captures the power spectrum of a sound.
- **Chroma**: Represents the energy of each pitch class.
- **Mel-Spectrogram**: Shows how the power of different frequencies is distributed over time.
- **Spectral Contrast**: Measures the difference in amplitude between peaks and valleys in a sound spectrum.
- **Zero-Crossing Rate (ZCR)**: Counts how often the signal crosses the zero amplitude axis.
- **Root Mean Square Energy (RMSE)**: Provides a measure of the signal's power.

## 🤖 Model Architecture

The SER model is built using a combination of CNN and LSTM layers:

- **Convolutional Layers**: Capture spatial hierarchies in the audio features.
- **LSTM Layers**: Capture temporal dependencies, crucial for sequential data like speech.
- **BatchNormalization**: Used to stabilize and accelerate training.
- **Dropout**: Added to prevent overfitting.

### 🙈 Model Summary:

- **Total Parameters**: 471,431
- **Trainable Parameters**: 470,535
- **Non-trainable Parameters**: 896

## 🏁 Results

### Torento Emotion Speech Set

- **Training Accuracy**: 98.99%
- **Validation Accuracy**: 98.2%

### Combined TESS, RAVDESS, and SAVEE Datasets

- **Training Accuracy**: 87%
- **Validation Accuracy**: 78%

## 🤔 How to Run

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/yourusername/speech-emotion-recognition.git
    cd speech-emotion-recognition
    ```

2. **Run the Speech emotion recognition file**: it will do the rest work
    ```bash
    Speech_Emotion_Recognition.ipynb
    ```

## Conclusion

This project demonstrates the power of combining CNNs and LSTMs for the task of speech emotion recognition. While the model performs exceptionally well on the Torento Emotion Speech Set, there is room for improvement when generalizing to a broader dataset. Future work could explore different architectures, feature engineering techniques, and data augmentation strategies.

## Acknowledgments

- **Kaggle** for providing the datasets.
- **Librosa** for the powerful audio processing tools.
- **Keras** for making model building accessible and intuitive.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
