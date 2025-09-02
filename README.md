# License Plate Recognition System

This project implements an License Plate Recognition (LPR) system using classical image processing and machine learning techniques in Python. The system detects license plates in car images, segments individual characters, and recognizes them using a trained Support Vector Machine (SVM) classifier.

## Features

- **License Plate Detection:** Locates license plates in car images using image thresholding and region properties.
- **Character Segmentation:** Extracts individual characters from the detected license plate.
- **Character Recognition:** Classifies segmented characters using an SVM trained on labeled character images.
- **Model Persistence:** Trained models are saved and can be reloaded for future predictions.

## Project Structure

```
LPRsystem.ipynb
requirements.txt
images/
    car.jpg
models/
    svc/
        svc.pkl
train/
    0/
    1/
    ...
    Z/
```

- `LPRsystem.ipynb`: Main Jupyter notebook containing the code for detection, segmentation, training, and prediction.
- `requirements.txt`: List of required Python packages.
- `images/`: Contains sample car images.
- `models/svc/`: Stores the trained SVM model.
- `train/`: Training images for each character (0-9, A-Z).

## Getting Started

### 1. Install Dependencies

Install the required Python packages:

```sh
pip install -r requirements.txt
```

### 2. Prepare Data

- Place your car images in the `images/` directory.
- Organize training images for each character in the `train/` directory (already structured).

### 3. Run the Notebook

Open `LPRsystem.ipynb` in Jupyter or VS Code and run all cells to:

- Detect and segment license plates and characters.
- Train the SVM model.
- Recognize characters from license plates.

### 4. Model Output

- The trained model is saved as `models/svc/svc.pkl`.
- The recognized license plate string is printed in the notebook output.

## Requirements

- Python 3.7+
- scikit-image
- numpy
- matplotlib
- scikit-learn
- pandas
- joblib

(See [`requirements.txt`](requirements.txt) for details.)

## Notes

- The system uses classical image processing; results may vary depending on image quality and plate styles.
- Training data should be 20x20 grayscale images for each character.
                         

**Author:**  
Mayank Sharma