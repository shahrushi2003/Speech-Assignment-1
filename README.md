# Spectrogram Analysis and Windowing Techniques Using UrbanSound8k Dataset

## Project Overview
This project demonstrates the application of different windowing techniques (Hann, Hamming, and Rectangular) for generating spectrograms from audio signals using the Short-Time Fourier Transform (STFT). The UrbanSound8k dataset was used for audio classification, where a Support Vector Machine (SVM) classifier was trained to evaluate the effectiveness of these windowing techniques.

## Dataset
**UrbanSound8k:** Contains 8,732 urban sound clips categorized into 10 classes.
- Download Link: [UrbanSound8k Dataset](https://goo.gl/8hY5ER)
- Metadata: UrbanSound8K.csv

## Project Structure
```
.
├── Ques2PartA.ipynb    # Notebook for spectrogram generation and classification
├── Ques2PartB.ipynb    # Additional spectrogram visualizations
└── README.md           # Project documentation (this file)
```

## Installation Instructions
### Dependencies
Ensure the following Python libraries are installed:
- `numpy`
- `librosa`
- `matplotlib`
- `scipy`
- `scikit-learn`
- `pandas`
- `tqdm`

### Installation
```bash
pip install numpy librosa matplotlib scipy scikit-learn pandas tqdm
```

## Usage
### Running the Analysis
1. **Ques2PartA.ipynb:**
   - Load the UrbanSound8k dataset and extract features using STFT with different windowing techniques.
   - Visualize spectrograms and train the SVM classifier.
   - Execute the cells in sequence for complete analysis.

2. **Ques2PartB.ipynb:**
   - Provides additional spectrogram visualizations using various music files for better understanding of STFT.

### Sample Commands
To plot spectrograms for different window types:
```python
plot_spectrogram(audio, sr, window_type='hann')
```
To train the SVM classifier:
```python
train_svc_model('hann')
```

## Results
| Window Type   | Accuracy | Precision | Recall | F1-Score |
|---------------|----------|-----------|--------|----------|
| Hann          | 70%      | 0.73      | 0.69   | 0.70     |
| Hamming       | 71%      | 0.74      | 0.70   | 0.71     |
| Rectangular   | 71%      | 0.74      | 0.70   | 0.71     |

## Conclusion
- Hann and Hamming windows provided better spectrogram visualizations and higher classification accuracy compared to the Rectangular window.
- The Hann window emerged as the most effective for minimizing spectral leakage.


## Author
Prepared for spectrogram analysis and windowing techniques assignment using UrbanSound8k dataset.

