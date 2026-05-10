# Image Segmentation for N/C Ratio Analysis

This project uses image segmentation to classify cell image pixels as background, cytoplasm, or nucleus. After generating segmentation masks, the notebook estimates the nucleus-to-cytoplasm ratio and compares different segmentation methods.

## Goal

Classify cell image pixels into three classes:

- Background
- Cytoplasm
- Nucleus

Then use the predicted masks to calculate the nucleus-to-cytoplasm ratio.

## Methods Compared

- Hand-picked thresholding
- Optimized thresholding
- Random Forest pixel classifier

## Evaluation Metrics

- Dice score for segmentation quality
- N/C Ratio MAE for measurement accuracy
- Predicted vs. true N/C ratio comparison
- Error distribution plots

## Main Result

The Random Forest pixel classifier achieved the lowest N/C ratio error on the held-out test set, while optimized thresholding achieved a similar Dice score. This showed that segmentation quality and final measurement accuracy are related, but not always identical.

## Tools Used

- Python
- NumPy
- pandas
- Matplotlib
- scikit-learn
- Google Colab

## Credit

Dataset and original lab materials were provided through the VocEd image segmentation lab repository. This notebook is my cleaned project version focused on comparing segmentation methods for nucleus-to-cytoplasm ratio estimation.
