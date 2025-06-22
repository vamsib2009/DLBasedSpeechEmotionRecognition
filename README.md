# DLBasedSpeechEmotionRecognition
CS5152 Deep Learning Project - Speech Emotion Recognition on IEMOCAP dataset

## Dataset
The IEMOCAP (Interactive Emotional Dyadic Motion Capture) dataset consists of 302 video segments from 5 sessions, with each session featuring a unique pair of speakers (total of 10 speakers). Each segment is annotated with 9 emotion labels — angry, excited, fear, sad, surprised, frustrated, happy, disappointed, and neutral — along with continuous attributes: valence, arousal, and dominance. The dataset supports multimodal emotion recognition, combining audio, video, and text data.

## Task: Speech Emotion Recognition
This project focuses on recognizing emotions from speech. The goal is to classify spoken utterances (from audio files) into the emotion categories.

## Novelty
Emotions impact how phonemes are expressed in speech. This project uses phonetic-level features from a Wave2Vec model to improve emotion recognition.

## Model Overview
![model_architecture (1)](https://github.com/user-attachments/assets/72d6eadd-2e41-424f-9c0a-aa20e250d700)

## Results
The proposed model achieved an accuracy of 78.97% on the IEMOCAP dataset, outperforming existing pure audio-based methods as of May 2024.
As of June 2025, the current state-of-the-art accuracy stands at 83.1%.

| Method                                            | Input       | Accuracy (%) |
| ------------------------------------------------- | ----------- | ------------ |
| ASR audio + word analysis (Xu et al.)             | Audio       | 70.6         |
| Feature Combine Attention + BiLSTM                | Audio       | 73.2         |
| Wave2Vec + FC                                     | Audio       | 78.15        |
| **Proposed Model (this work)**                    | Audio       | **78.97**    |
| VMD + Energy-Based Adaptive Mode Selection (2025) | Audio       | **83.1**     |









