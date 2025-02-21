# Multimodal Environment Classification

## Introduction
This project is designed to analyze and classify environments using **multimodal data** (images and audio). It is implemented in **Jupyter Notebook** to provide an interactive environment for data analysis and visualization. The goal is to demonstrate the potential of multimodal approaches in improving classification accuracy compared to using only a single data type (images or audio).

## About the Dataset
### Data Source
The dataset consists of **images** obtained from **8 different environment types**, along with **audio files** corresponding to these images. The data was extracted from **37 video recordings**, with each second of video represented by an image and **MFCC (Mel-Frequency Cepstral Coefficients)** statistics for the corresponding audio segment.

### Key Points
- **Images** are extracted at 1-second intervals (frames at 0.5s, 1.5s, 2.5s, etc.).
- **Each image** is accompanied by a set of **MFCC audio attributes** calculated for the corresponding second of video.

### Problem Statement
- **London Video:** The visual classifier incorrectly identifies the environment as "FOREST" when a woman with flowing hair walks by.
- **Las Vegas Video:** The audio classifier confuses "CITY" with "RIVER" due to the sound of a large fountain.
- **Solution:** The multimodal approach helps eliminate such errors by combining image and audio data.

## Data Format
The dataset is provided in `dataset.csv`. Each row contains:
- **Path to the image**
- **104 MFCC attributes** derived from audio (13 coefficients across 8 time windows)

### Classification Tasks
- **Binary Classification:** "Indoors" vs. "Outdoors"
- **Multiclass Classification:** 8 different environment types

## Project Objectives
- Analyze the impact of the **multimodal approach** on environment classification.
- Explore **data characteristics** and demonstrate steps for **analysis and preprocessing**.
- Develop a **classification methodology** using images, audio, and their combination.

## Technologies Used
- **Programming Language:** Python
- **Development Environment:** Jupyter Notebook
- **Libraries:** Pandas, NumPy, Matplotlib, Scikit-learn, OpenCV, Librosa

## Project Structure
1. **Data Loading and Preliminary Analysis:**
   - Analyze dataset format and visualize class distribution.
2. **Image Processing:**
   - Preprocess and prepare image data for training.
3. **Audio Data Processing:**
   - Analyze **MFCC attributes**, normalize, and prepare data.
4. **Multimodal Classification:**
   - Combine **image and audio data** to build classification models.
5. **Evaluation of Results:**
   - Compare classification accuracy using single modalities vs. multimodal approaches.

## Citation
Dataset Source: [Kaggle Scene Classification - Images and Audio](https://www.kaggle.com/datasets/birdy654/scene-classification-images-and-audio/)

## Conclusion
This project demonstrates how a **multimodal approach** can enhance environment classification accuracy by addressing errors common in **single-modality classifiers**. The approach can be adapted for other **multimodal research tasks and datasets**.

## Author
Farukh Rustamov
