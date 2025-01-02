# CNN-on-CIFAR10-Image-Classification
This project demonstrates the application of a 3-layer Convolutional Neural Network (CNN) for end-to-end image classification on the CIFAR-10 dataset. The CNN is trained directly on raw image data without any prior dimensionality reduction.

## Key Features
- **Dataset**: Utilizes the CIFAR-10 dataset containing 60,000 32x32 color images across 10 classes.
- **Architecture**: Implements a 3-layer CNN designed for feature extraction and classification.
- **Evaluation Metrics**: Accuracy, precision, recall, and F1-score are used to evaluate model performance.

## Highlights
- Directly processes raw image data without any preprocessing like PCA.
- Achieves competitive classification performance with a carefully designed 3-layer CNN.
- Includes visualizations of training and validation metrics, such as accuracy and loss.

## Hyperparameter Tuning
Hyperparameter tuning was performed to optimize the CNN’s performance:
- **Learning Rates**: Tested values in the set {0.001, 0.01, 0.1}.
- **Batch Sizes**: Evaluated batch sizes of 8, 16, 32 and 64.
- **Number of Convolutional filters**: Experimented with {8, 16, 32}
- **Dropout rate**: Experimented dropout rates of 0.2 and 0.5.

The best configuration achieved a classification accuracy of **90.12%** and an AUROC of **96.02%** on the test set.

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/BrightManu/CNN-on-CIFAR10-Image-Classification.git
   ```
2. Install dependencies:
   ```bash
   pip install numpy matplotlib torch torchvision
   ```
3. Open the notebook:
   - Launch Jupyter Notebook or any compatible environment.
   - Open the notebook file (`CNN_CIFAR10.ipynb`).
4. Execute all cells sequentially to run the project.

## Acknowledgments
CIFAR-10 Dataset: [CIFAR-10](https://www.cs.toronto.edu/~kriz/cifar.html)
