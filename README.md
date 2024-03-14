# Chord Recognition Algorithm

Algorithm aimed at identifying the underlying musical chords within an audio signal.

## Overview:

This repository contains an implementation of a chord recognition algorithm based on chromagrams and predefined chord templates. The algorithm processes audio files in WAV format, computes chromagrams, calculates cosine similarity with templates, and identifies chord labels.

## Features:

- **Chromagram Computation**: Utilizes Short-Time Fourier Transform (STFT) to compute chromagrams from audio signals.
- **Template Matching**: Compares chromagrams with predefined chord templates using cosine similarity.
- **Preprocessing**: Includes normalization, smoothing, and downsampling techniques for enhancing chord recognition accuracy.
- **CSV Ground Truth Data Preprocessing**: Converts segment-based annotations into frame-based sequences and standardizes chord labels for evaluation.

## Usage:

1. **Input Audio Files**: Place the audio files you wish to analyze in the `data/wav/` directory.
2. **CSV Ground Truth Data**: Provide CSV files with ground truth chord annotations in the `data/csv/` directory.
3. **Run Algorithm**: Execute the chord recognition algorithm by calling the `complete_function()` function with appropriate parameters.
4. **Evaluate Accuracy**: Evaluate the accuracy of the algorithm using the provided ground truth data and the `metrics()` function.

## Dependencies:

- Python 3.x
- NumPy
- Librosa
- Pandas
- Matplotlib
- Scikit-learn
- SciPy

