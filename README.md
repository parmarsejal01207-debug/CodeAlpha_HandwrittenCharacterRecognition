
# CodeAlpha_HandwrittenCharacterRecognition
Machine Learning Internship at CodeAlpha, Task 3: Handwritten Character Recognition.

## Objective
Recognize handwritten digits (0-9) from images using a Convolutional Neural Network (CNN).

## Dataset
MNIST dataset, loaded via Keras.
- 60,000 training images and 10,000 test images
- Each image is 28x28 pixels, grayscale
- 10 classes (digits 0 to 9)

## Approach
1. Load and visualize the dataset
2. Preprocess: normalize pixels to 0-1 and reshape to (28, 28, 1)
3. Build a CNN: 2 x (Conv2D + MaxPooling), Flatten, Dropout (0.3), Dense (128), Softmax (10)
4. Train for 5 epochs (Adam optimizer, batch size 128, 10% validation split)
5. Evaluate with accuracy, confusion matrix and classification report

## Results

| Metric               | Value  |
|----------------------|--------|
| Test Accuracy        | 99.03% |
| Test Loss            | 0.0290 |
| Final Train Accuracy | 98.88% |
| Final Val Accuracy   | 99.10% |

Precision, recall and F1-score are about 0.98-1.00 for every digit.

## Conclusion
- The CNN reached **99.03% test accuracy** in only 5 epochs, with no sign of overfitting.
- Digit 9 had the lowest recall (0.97), mostly confused with 7 and 8.
- CNN is well suited for image recognition as it learns edges and shapes automatically.

## Tech Stack
Python, TensorFlow/Keras, NumPy, Scikit-learn, Matplotlib, Seaborn, Jupyter Notebook

## How to Run
1. Install the libraries: `pip install tensorflow scikit-learn matplotlib seaborn jupyter`
2. Open the notebook: `jupyter notebook CodeAlpha_Task3_HandwrittenRecognition.ipynb`
3. Run all cells (Kernel, then Restart & Run All)

## Author
Parmar Sejal, Machine Learning Intern at CodeAlpha
