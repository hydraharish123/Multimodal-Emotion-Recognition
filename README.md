## Multimodal Emotion Recognition from Speech and Transcripts

This project implements a deep learning pipeline for emotion recognition using both audio signals and text transcripts. It fuses features from **spectrogram-based CNN** and **LSTM-based text processing** to improve emotion classification on the RAVDESS dataset.

### 📁 Project Structure

```
.
├── Audio                                      # Contains the input files from RAVDESS dataset  # File size too large to upload on github
├── MultiModalEmotionRecognition.ipynb         # Code implementation with explanation
├── requirements.txt                           # Libraries used for this project
├── spectrograms                               # Spectrograms obtained while training CNN       # File size too large to upload on github
└── README.md
```

### 📊 Results

| Model                     | Validation Accuracy        |
| ------------------------- | -------------------------- |
| CNN (Audio Spectrograms)  | 76%                        |
| LSTM (Text Transcripts)   | 16%                        |
| Early Fusion (CNN + LSTM) | **57%** (at 10 epochs) |

Fusion improves over unimodal text classification significantly, even though it doesn’t yet surpass audio-only performance.

### Features

* Spectrogram generation using Librosa
* CNN for image-based classification
* LSTM for text-based classification
* Early fusion of audio and text features


### Requirements

Install dependencies with:

```bash
pip install -r requirements.txt
```

### 📚 Dataset

This project uses the [RAVDESS dataset](https://www.kaggle.com/datasets/uwrfkaggler/ravdess-emotional-speech-audio), which includes speech recordings with emotional labeling.

---

