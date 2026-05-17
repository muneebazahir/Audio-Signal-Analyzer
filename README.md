# Audio Signal Analysis, Convolution & Rule-Based Language Identification (MATLAB GUI)

A MATLAB-based Digital Signal Processing (DSP) project that performs:

- Audio signal analysis  
- Rule-based language identification (English/French)  
- Linear convolution of audio signals  
- Audio playback and saving  
- Interactive GUI operations using MATLAB App Designer  

---

##  Project Overview

This application allows users to:

Load and analyze speech audio signals  
Extract DSP features such as:
- Zero Crossing Rate (ZCR)
- Spectral Centroid
- Pitch
- Energy

Detect language using rule-based heuristics (without Machine Learning)  
Perform convolution between two audio signals  
Play and save the convolved output  
Interact through a user-friendly MATLAB GUI  

---

##  Language Detection Logic

The system uses simple DSP-based rules for classification:

- **Higher ZCR + Higher Spectral Centroid → Likely French**
- **Lower ZCR + Stable Pitch → Likely English**

> Note: This is a heuristic/rule-based approximation and not a machine learning model.

---

## Technologies Used

- MATLAB
- MATLAB App Designer
- Digital Signal Processing Techniques
- Audio Feature Extraction
- GUI Development

---

##  Features

###  Audio Signal Processing
- Load `.wav` audio files
- Convert stereo audio to mono
- Normalize signals

###  Feature Extraction
The project extracts:
- Zero Crossing Rate (ZCR)
- Spectral Centroid
- Pitch
- Signal Energy

###  Rule-Based Language Detection
Uses threshold conditions based on extracted audio features.

###  Signal Convolution
- Load second signal
- Apply linear convolution using `conv()`
- Normalize output signal

###  Playback & Saving
- Play processed audio
- Save output using `audiowrite()`

###  MATLAB GUI
Interactive GUI buttons:
- Load Audio
- Extract Features
- Detect Language
- Load Second Signal
- Convolve
- Play Output

---

## How to Run the Project

### Requirements
- MATLAB R2021a or later
- Signal Processing Toolbox
- Audio Toolbox (recommended)

### Steps
1. Clone this repository:

```bash
https://github.com/muneebazahir/Audio-Signal-Analyzer
```

2. Open MATLAB.

3. Open the `.mlapp` file in App Designer.

4. Run the application.

5. Load audio files and test the features.

---

##  Project Structure

```plaintext
├── DSP_Project.mlapp
├── README.md
├── sample_audio/
├── output/
├── images/
└── report/
```

---

## DSP Concepts Used

### Audio Representation

```math
x[n]
```

### Linear Convolution

```math
y[n] = x[n] * h[n] = \sum_{k=-\infty}^{\infty} x[k]h[n-k]
```

Applications:
- Filtering
- Echo/Reverb Simulation
- Signal Processing

---

## Learning Outcomes

This project helps in understanding:

- DSP fundamentals
- Feature extraction techniques
- Rule-based classification
- Signal convolution
- MATLAB GUI development
- Real-world audio signal analysis

---

## Author

**Muneeba Zahir**  
 Computer Engineer

---

## Academic Note

This project was developed for educational purposes as part of the DSP Lab coursework.  
The implementation follows a **rule-based approach only** and does not use Machine Learning algorithms.

---

## License

This project is intended for educational and learning purposes only.
