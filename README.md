# Speech Emotion Recognition

collabrated with [Tarun Raman](https://github.com/2307tarun)
  
  - Implemented a NLP pipeline to classify emotions into eight classes and detect the gender of the speaker using the RAVDESS dataset.
  -  Trained and compared DL models MLP and CNN on audio features extracted like MFCC, Chroma, Spectral Rolloff, Mel and ZCR Voice using the Librosa library.
  -   Achieved test accuracy of 68% on emotion classification and ∼99.3% on gender classification using MLP architecture.
  -   CNN and LSTM Models are being worked upon.

## Abstract
Detection of emotions is natural for humans, but it is a very difficult task for computers, since accessing the depth behind content is difficult and that’s what speech emotion recognition (SER) sets out to do. It is a system through which various audio speech files are classified into different emotions such as happy, sad, anger and neutral by computers.

## Dataset
The RAVDESS is a validated multimodal database of emotional speech and song. The database is gender balanced consisting of 24 professional actors, vocalizing lexically-matched statements in a neutral North American accent. Speech includes calm, happy, sad, angry, fearful, surprise, and disgust expressions, and song contains calm, happy, sad, angry, and fearful emotions. All conditions are available in face-and-voice, face-only, and voice-only formats.

## Feature Extraction
Feature extraction is important in modeling because it converts audio files into a format that can be understood by models.

1. MFCC (Mel-Frequency Cepstral Coefficients)- It is a representation of the short-term power spectrum of a sound, based on linear cosine transformation of a log power spectrum on nonlinear mel frequency scale.
2. Chroma- It closely relates to the 12 different pitch classes. It captures harmonic and melodic characteristics of music.
3. Mel Scale- It is a perceptual scale of pitches judged by listeners to be in equal in distance from one another. 
4. Zero Crossing Rate (ZCR)- It is the rate at which a signal changes from positive to zero to negative or from negative to zero to positive.
5. Spectral Centroid- It is the center of 'gravity' of the spectrum. It is a measure used in digital signal processing to characterize a spectrum.

 ## Model Implementation

**MLP (Multi-Layer Perceptron) Model:**
The  arrays containing features of the audios are given as an input to the MLP Classifier that has been  initialized. The Classifier identifies different categories in the datasets  and classifies them into different emotions.

**Convolutional Neural Network (CNN):**
The activation layer called as the RELU layer is  followed by the pooling layer. The specificity of the CNN layer is  learnt from the functions of the activation layer. 

**RNN-LSTM Model:**
We used RMSProp optimizer to train the RNN-LSTM model, all  the experiments were carried with a fixed learning rate. Batch  Normalization is applied over every layer and the  activation function used is the SoftMax activation function.
