# Image Edge Detection Comparison

A Python script using OpenCV and Matplotlib to compare three classical edge detection algorithms—**Sobel**, **Prewitt**, and **Canny**—against an original grayscale image.

---

## Overview

Edge detection is a fundamental technique in computer vision used to identify sharp brightness changes in an image. This project implements and visualizes three distinct approaches:

* **Sobel Filter:** Computes image gradients using Gaussian smoothing combined with differentiation to reduce high-frequency noise.
* **Prewitt Filter:** Uses discrete gradient operator matrices to calculate magnitude approximations of edge intensity.
* **Canny Edge Detector:** A multi-stage algorithm that uses noise reduction, intensity gradient computation, non-maximum suppression, and hysteresis thresholding to extract clean, thin edges.

---

## Output Comparison

The script generates a $2 \times 2$ grid displaying the visual results side-by-side:

| Method | Characteristics | Best For |
| :--- | :--- | :--- |
| **Original** | Base input converted to single-channel grayscale. | Reference |
| **Sobel** | Emphasizes edges with Gaussian smoothing; continuous gradient intensity. | General gradient analysis |
| **Prewitt** | Computes horizontal/vertical gradient components directly. | Fast edge detection |
| **Canny** | Thin, sharp single-pixel edges with noise removal via hysteresis. | Structural segmentation |

---

## Requirements

Ensure you have Python 3.x and the required libraries installed:

```bash
pip install opencv-python numpy matplotlib
