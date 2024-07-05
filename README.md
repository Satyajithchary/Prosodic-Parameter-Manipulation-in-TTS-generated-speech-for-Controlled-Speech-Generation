# 🎤 Prosodic Parameter Manipulation in TTS Generated Speech for Controlled Speech Generation

This repository contains the code and resources for the project **"Prosodic Parameter Manipulation in TTS Generated Speech for Controlled Speech Generation."** This project aims to improve the naturalness and expressiveness of TTS-generated speech by manipulating prosodic parameters. And this project is done as a part of IASNLP - 2024 at LTRC LAB, IIIT Hyderabad

## 📚 Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Methodology](#methodology)
- [Results](#results)
- [Future Scope](#future-scope)
- [References](#references)
- [Usage](#usage)

## 🎯 Introduction

The goal of this project is to enhance the naturalness of TTS-generated speech by adjusting prosodic parameters such as pitch (F0), duration, and intensity. By modifying these parameters, we aim to produce speech that is more expressive and closer to natural human speech.

## 📊 Dataset

The datasets used in this project include both original human speech recordings and TTS-generated speech. These datasets are organized as follows:

- **Original Human Speech**:
  - Italian: `/content/drive/MyDrive/data (1)/data/wav/ITA/train`
  - German: `/content/drive/MyDrive/data (1)/data/wav/GER/train`
- **TTS-Generated Speech**:
  - Italian: `/content/drive/MyDrive/Audio_Files/ITA_Train_TTS_Audios`
  - German: `/content/drive/MyDrive/Audio_Files/GER_Train_TTS_Audios`

Additional data for stress patterns in speech is provided in:
- Italian stress training: `/content/ITA_train.xlsx`
- German stress training: `/content/GER_train.xlsx`

## ⚙️ Methodology

The methodology involves several steps:
1. **Data Preprocessing**: Convert audio files to a suitable format for analysis.
2. **Prosodic Feature Extraction**: Extract features such as pitch (F0), duration, and intensity from the audio files.
3. **Prosodic Parameter Manipulation**: Modify the extracted prosodic parameters to achieve desired speech characteristics.
4. **Re-synthesis**: Generate modified speech using the manipulated prosodic parameters.
5. **Evaluation**: Compare the modified speech with the original to evaluate the effectiveness of the manipulations.

The main steps in the code are as follows:
- Extract and manipulate F0 using `pyworld`.
- Modify duration and intensity based on prosodic patterns.
- Re-synthesize the modified speech using `pydub`.

## 📈 Results

The results show significant improvements in the naturalness of TTS-generated speech. The following figures illustrate the comparison between original and modified F0 contours and spectral envelopes:

### Figure 1: F0 Comparison for Sample 1
![F0 Comparison for Sample 1](https://github.com/Satyajithchary/Prosodic-Parameter-Manipulation-in-TTS-generated-speech-for-Controlled-Speech-Generation/blob/main/Output_Files/ISLE_SESS0003_BLOCKD01_09_sprt1_f0_comparison.png?raw=true)


### Figure 2: F0 Comparison for Sample 2
![F0 Comparison for Sample 2](https://github.com/Satyajithchary/Prosodic-Parameter-Manipulation-in-TTS-generated-speech-for-Controlled-Speech-Generation/blob/main/Output_Files/ISLE_SESS0003_BLOCKD01_07_sprt1_f0_comparison.png?raw=true)

### Figure 3: Spectral Envelope Comparison for Sample 3
![Spectral Envelope Comparison for Sample 3](https://github.com/Satyajithchary/Prosodic-Parameter-Manipulation-in-TTS-generated-speech-for-Controlled-Speech-Generation/blob/main/Output_Files/ISLE_SESS0003_BLOCKD01_06_sprt1_adjusted_audio_spectral_envelope_comparison.png?raw=true)

## 🔮 Future Scope

Future work could involve:
- Extending the methodology to other languages and dialects.
- Incorporating more sophisticated models for prosodic parameter manipulation.
- Improving the evaluation metrics to include subjective listening tests.

## 📚 References

- [pyworld](https://github.com/JeremyCCHsu/Python-Wrapper-for-World-Vocoder)
- [pydub](https://github.com/jiaaro/pydub)

## 🚀 Usage

To use this code, follow these steps:

1. **Clone the repository:**

```bash
git clone (https://github.com/Satyajithchary/Prosodic-Parameter-Manipulation-in-TTS-generated-speech-for-Controlled-Speech-Generation)
```

2. **Navigate to the project directory:**

```bash
cd Prosodic-Parameter-Manipulation-in-TTS-generated-speech-for-Controlled-Speech-Generation
```

3. **Install the required dependencies:**

```bash
pip install -r requirements.txt
```

4. **Run the main script:**

```bash
python main.py
```

5. **View the results:**

The results will be saved in the specified output directory, including modified audio files and comparison plots.
