# Vowel Detector

## Introduction
This project is a practical exercise from my Digital Signal Processing course, focusing on three different tasks related to digital signal processing and the spectral characteristics of vowels. Our group achieved perfect scores due to high accuracy and strong presentation skills.

### Assignment 1: Spectral Feature Analysis of Vowels
- **Input**: Voice signals.
- **Output**:
  - Spectrogram images and the triad of formant frequencies {F1, F2, F3} for each vowel, marked directly on the spectrogram.
  - Observations on the spectral characteristic differences among various vowels of the same speaker.
- **Requirements**:
  - Generate wideband spectrograms for training files (selected randomly from 21 speakers in the 'NguyenAmHuanLuyen-16k' directory).
  - Present a table or spectrogram annotations of the formant frequencies for each vowel and provide insights into the spectral differences among the five vowels of one speaker from the selected four.

### Assignment 2: Speaker-Independent Vowel Recognition Using FFT Spectral Features
- **Input**: Voice signals (containing one vowel and silence) from the test set ('NguyenAmKiemThu-16k' with 21 speakers, 105 test files).
- **Output**:
  - Identification results (predicted vowel labels /a/, …,/u/), Correct/Incorrect (based on file name labels).
  - Five feature vectors representing five vowels on a single graph.
  - Statistical accuracy (%) based on the feature vector's dimension (number of frequency domain sampling points N_FFT with values 512, 1024, 2048).
  - Confusion matrix for the highest accuracy scenario among the three N_FFT values.

### Assignment 3: Speaker-Independent Vowel Recognition Using MFCC Spectral Features
- **Input**: Voice signals (containing one vowel and silence) from the test set (21 speakers, 105 test files).
- **Output**:
  - Identification results (predicted vowel labels /a/, …,/u/), Correct/Incorrect (based on file name labels).
  - Five MFCC feature vectors representing five vowels on a single graph.
  - Overall identification accuracy (%) based on the number of MFCC feature vector dimensions (N_MFCC fixed at 13) and K (number of clusters with values 2, 3, 4, 5).

For detailed descriptions of the assignments, refer to: [Problem-Summary](https://github.com/tranductri2003/vowel-detector/blob/main/Y%C3%AAu%20c%E1%BA%A7u%20BT%20nh%C3%B3m%20-%20Ph%C3%A2n%20t%C3%ADch%20ph%E1%BB%95%20v%C3%A0%20nh%E1%BA%ADn%20d%E1%BA%A1ng%20t%C3%ADn%20hi%E1%BB%87u%20nguy%C3%AAn%20%C3%A2m_UPDATE%20(1).pdf).

## Our Results
### Assignment 1:
- Spectrogram for file 23MTL:
![Spectrogram 23MTL](https://github.com/tranductri2003/vowel-detector/assets/89126960/9c60e997-2a9f-486f-9ba8-0affc067b937)
- Spectrogram for vowel 'a':
![Spectrogram Vowel 'a'](https://github.com/tranductri2003/vowel-detector/assets/89126960/aa4fc878-fe55-4d11-b7f5-08db723d62c2)
- Triad of formant frequencies:
![Formant Frequencies](https://github.com/tranductri2003/vowel-detector/assets/89126960/b406718f-ebb7-4024-b538-b97fd1e09981)

### Assignment 2:
- Achieved 91% accuracy in vowel recognition using FFT spectral analysis.
- Feature vector representation of five vowels:
![Feature Vectors](https://github.com/tranductri2003/vowel-detector/assets/89126960/78d0e969-ac7f-4f18-a68d-77165ba37732)
- Confusion matrix:
![Confusion Matrix](https://github.com/tranductri2003/vowel-detector/assets/89126960/b15f8bde-c603-46e8-9b9f-78b8c7acab5b)
- Validation matrix:
![Validation Matrix](https://github.com/tranductri2003/vowel-detector/assets/89126960/fb5b297d-55bb-4477-baed-b53c7727ac8c)

### Assignment 3:
- Achieved 94% accuracy in vowel recognition using MFCC spectral features and K-Mean clustering with K=2.
- MFCC feature vectors for five vowels:
![MFCC Vectors](https://github.com/tranductri2003/vowel-detector/assets/89126960/02928b29-141a-4223-b581-c1445b9ff2a0)
- Inertia graph for different K values:
![Inertia Graph](https://github.com/tranductri2003/vowel-detector/assets/89126960/3430adf8-63f4-49ea-8f1e-dea3f4a3b7a0)
- Confusion matrix:
![Confusion Matrix](https://github.com/tranductri2003/vowel-detector/assets/89126960/5f6981db-c145-4f23-a73e-6de139937d10)

Detailed information can be found in the [Technical Report](https://github.com/tranductri2003/vowel-detector/blob/main/%5BSLIDE-Nhom14-XuLiTinHieuSo%5D.pdf).

## Installation
The source code for the above assignments, complete with detailed comments, is available for running and verification. Feel free to contact me with any questions.
- [Problem-1](https://github.com/tranductri2003/vowel-detector/blob/main/problem-1.ipynb)
- [Problem-2](https://github.com/tranductri2003/vowel-detector/blob/main/problem-2.ipynb)
- [Problem-3](https://github.com/tranductri2003/vowel-detector/blob/main/problem-3.ipynb)
