
# Plastic Object Classifier

**Plastic Object Classifier** is a deep learning project that automatically identifies the type of plastic from an image and suggests which conveyor belt it should go to for sorting. It classifies images into three categories: `black`, `colorful`, and `transparent`. The project is designed to demonstrate practical applications of image classification using a small, self-made dataset of 100 images per class.

---

## Project Overview

Sorting plastics manually is time-consuming and error-prone. This project automates the classification process using a Convolutional Neural Network (CNN). The model is trained on images of different types of plastic and learns to distinguish between them based on color and visual features. Once an image is analyzed, the system outputs:

* The detected type of plastic
* The confidence of the prediction
* The conveyor belt it should be sent to

This workflow mimics a real-world sorting system, showing how machine learning can assist in automation and recycling processes.

---

## Features

* **Image Classification:** Automatically detects plastic type from images
* **Conveyor Assignment:** Recommends which conveyor belt each plastic item should go to
* **Self-Made Dataset:** 100 images per class for demonstration purposes
* **Simple Workflow:** Easy to run and understand, suitable for small datasets

---

## Project Structure

* `plastic_classifier.py` — Main script for training the model and predicting new images
* `dataset/` — Training images organized into `black`, `colorful`, and `transparent` folders
* `requirements.txt` — List of Python packages required

---

## Dataset Download

The dataset is **hosted externally** due to file size. Download it from Google Drive:

[Download Dataset](https://drive.google.com/drive/folders/16ubaEOjQUHwLbgHZBgxp8vp8o8jJJ3MB?usp=sharing)

After downloading, **unzip the dataset** into a folder named `dataset` in the project root. The structure should look like this:

```
dataset/
   black/
   colorful/
   transparent/
```

---

## Requirements

Install the required Python packages using:

```
pip install -r requirements.txt
```

Dependencies include: tensorflow, numpy, scikit-learn, Pillow

---

## Usage

1. Download and unzip the dataset as explained above.
2. Run the script:

```
python plastic_classifier.py
```

3. Provide a new image for prediction.
4. The system outputs:

   * Detected plastic type
   * Confidence percentage
   * Recommended conveyor belt

---

## Notes

* The dataset is large (~488 MB) and hosted externally; the project is intended for demonstration and learning purposes.
* All file paths in the script are relative, so the project runs immediately after setting up the dataset.
* The model is simple but illustrates how image classification can be applied to practical problems like recycling automation.

