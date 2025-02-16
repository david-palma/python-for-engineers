# Automated wear analysis of a gear

This exercise explores the application of computational techniques to analyse wear on gear teeth using image processing methods in Python. Gears are fundamental components in mechanical systems, but prolonged operation can lead to wear, compromising efficiency and service life. Wear analysis is essential for maintaining machinery reliability, as degradation can cause performance loss, increased vibration, and potential mechanical failure. This study focuses on developing a method to detect and quantify wear by analysing gear images, extracting key features from the gear’s contour, and comparing them to a reference gear in pristine condition. Automating this process enhances accuracy, reduces manual inspection efforts, and supports predictive maintenance strategies.

## Objectives

The primary objectives of this exercise are:

1. **Image acquisition**: Load an image of a gear captured under controlled conditions with a uniform background to facilitate analysis.

2. **Pre-processing and noise reduction**: Enhance the image quality by reducing noise and improving the segmentation of the gear's contour.

3. **Contour detection**: Extract the outer contour of the gear to isolate its structure for further analysis.

4. **Key point detection**: Identify key points along the gear’s contour that correspond to the vertices of its teeth, providing the basis for wear assessment.

5. **Wear analysis**: Compare the identified key points with those of a reference image of a perfect gear to detect deviations indicative of wear.

## Methodology

The analysis follows a systematic workflow:

1. **Data preparation**:
    - Two test images are provided: a reference image of a perfect gear (`data/gear.jpg`) and an image of a worn gear (`data/worn_gear.jpg`). These serve as inputs for the system.

2. **Image pre-processing**:
    - Convert the input image to grayscale to simplify processing.
    - Apply filters to reduce noise and emphasise the gear's contour for accurate segmentation.

3. **Contour extraction**:
    - Detect the gear's outer contour using edge detection algorithms.
    - Isolate the contour to identify the gear's boundaries and prepare for key point detection.

4. **Key point detection**:
    - Extract key points along the contour that represent the vertices of the gear teeth.
    - Use these points to define the geometry of the gear and its teeth.

5. **Wear analysis**:
    - Compare the positions of the key points from the test image to those of the reference gear image.
    - Quantify deviations to detect and measure wear on the gear teeth.

## Testing the system

The system is tested with the following images:

1. **Perfect gear image** (`data/gear.jpg`): Represents a gear in optimal condition with no visible wear. This serves as a reference for the analysis.

2. **Worn gear image** (`data/worn_gear.jpg`): Depicts a gear with visible wear on its teeth, enabling the system to demonstrate its ability to detect and quantify wear.

To test the system, users can modify the filename in the provided Jupyter notebook to select the image they wish to analyse. Customisation options allow users to experiment with different parameters, such as noise reduction filters and key point detection thresholds, to observe their impact on the analysis.

---

This exercise highlights the potential of automated image processing for industrial maintenance. By streamlining the wear detection process, the methodology supports predictive maintenance strategies, reduces operational downtime, and enhances machinery reliability.
