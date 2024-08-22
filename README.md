# Distinguishing-AI-Generated-and-Human-Written-Scientific-Texts-

## Introduction

This project focuses on distinguishing AI-generated and human-written scientific texts using machine learning techniques. The core of this work involves two main components: a feature extraction model and a Support Vector Machine (SVM) classifier. This work was part of the course Human Language Technologies (HLT), lectured by Prof. Stapparava Carlo @unitn. It is part of my final exam submission.

## Data
The necessary data is stored as a shared folder on my GoogleDrive: https://drive.google.com/drive/folders/1-4G44bGfXkh85DPWaFzT0gIM5282CE7C?usp=sharing

## Feature Extraction Model

The feature extraction model is designed to analyze textual data and derive various linguistic features. These features, which include both regex-based and statistical metrics, are used to capture distinctive patterns and structures in the text that might indicate whether a text is AI-generated or human-written.

### Key Features Extracted:
- **Regex-Based Features:** Detection of specific punctuation marks, use of connectors, and certain key terms that might reflect stylistic choices.
- **Statistical Features:** Measures such as sentence length standard deviation, word count, and lexical diversity.

The feature extraction model was inspired by the work of Desaire et al., who originally implemented a similar model in R. Their approach served as a foundation for developing the feature extraction scripts used in this project.

**Credits:** The original concept and R code for feature extraction were derived from Desaire et al., as detailed in their paper *"Distinguishing academic science writing from humans or ChatGPT with over 99% accuracy using off-the-shelf machine learning tools"* (Cell Reports Physical Science, 2023), https://doi.org/10.1016/j.xcrp.2023.101426. 

## Classifier (SVM)

After extracting the relevant features, the next step involves classifying the text as either AI-generated or human-written. This is accomplished using a Support Vector Machine (SVM), a robust classifier well-suited for binary classification tasks. The SVM is trained on the extracted features, learning to distinguish between the two classes with high accuracy.


## Conclusion

This project provides a powerful toolset for distinguishing between AI-generated and human-written scientific texts. While the models perform well in controlled scenarios, further work is needed to generalize these results to more varied and less controlled environments.

**Note:** Please refer to the original paper by Desaire et al. for a detailed understanding of the feature extraction model and its underlying principles.
