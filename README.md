# Masters Thesis

# Denoising Doppler Spectra with Residual Convolutional Autoencoder

This repository contains the implementation of a **Residual Convolutional Autoencoder (CAE)** for denoising Doppler power spectra from the Davis MST radar, as part of an M.Tech project. The project introduces a novel CAE with residual connections and a spectral loss function to improve signal-to-noise ratio (SNR) and preserve spectral features critical for atmospheric wind parameter estimation.

## Project Overview

The goal is to denoise Doppler power spectra from the Davis Mesosphere-Stratosphere-Troposphere (MST) radar, stored in .dbs format (DBS_messo and DBS_tropo datasets). The proposed residual CAE enhances denoising performance compared to traditional methods like Wiener filtering and wavelet denoising, achieving superior SNR and peak preservation for radar signal processing.

### Key Features
- **Residual CAE**: A convolutional autoencoder with residual connections for improved training stability and denoising performance.
- **Spectral Loss Function**: A custom loss that preserves spectral peaks, tailored for Doppler spectra.
- **Dataset**: Processes .dbs files from Davis MST radar (1900 KB for DBS_messo, 800 KB for DBS_tropo).
- **Evaluation**: Metrics include SNR, MSE, and peak preservation error, with comparisons against Wiener filtering, wavelet denoising, and a baseline CAE.
