# Neural Networks Project: Calibration of CNNs for Bird-Cat Classification

**Credit:**
The implementation is based on tasks provided by Pablo M. Olmos.

**Completed by:**
- **Marina Gómez Rey** (https://github.com/MarinaGRey)
- **Ángela Durán**
- **María Ángeles Magro Garrote**

## Abstract
This project investigates the calibration of convolutional neural networks (CNNs) in a classification setting, focusing on distinguishing birds from cats in the CIFAR-10 dataset. The project includes:
1. A review of neural network calibration techniques, based on the paper "On Calibration of Modern Neural Networks."
2. Training a LeNet-5 CNN from scratch and assessing its calibration using reliability diagrams and Expected Calibration Error (ECE).
3. Implementing temperature scaling (Platt's scaling) to refine model output probabilities, optimizing the temperature parameter.
4. Comparing performance with a fine-tuned DenseNet model, which involves modifying a pre-trained model for the CIFAR-10 dataset.

## Creation of the Model
The project employs the LeNet-5 architecture, characterized by:
- **Input Size**: 32x32 CIFAR-10 images.
- **Architecture**: Two convolutional layers with 5x5 filters, followed by max-pooling layers with 2x2 kernels, and three fully connected layers.
- **Early Stopping**: Applied to prevent overfitting during training.

## Reliability Diagram & ECE
- **Reliability Diagram**: A graphical tool for comparing mean predicted probabilities with empirical probabilities, used to evaluate model calibration.
- **Expected Calibration Error (ECE)**: A metric for measuring calibration error, which helps in assessing and comparing the quality of model calibration.

## Calibration
- **Temperature Scaling (Platt's Scaling)**: Adjusts the model's output probabilities to align more closely with true probabilities. This includes optimizing the temperature parameter and evaluating its impact on calibration.

## Big Model
- **Fine-Tuning DenseNet**: Adapts a pre-trained DenseNet model for the CIFAR-10 dataset, including resizing input images and applying data augmentation. The final classifier layer is modified to fit the classification task.

## Files
- `Report.pdf`: Comprehensive report detailing the project's methodology, experiments, and findings.
- `Code.ipybn`: Jupyter notebook containing the code used for implementing and evaluating the models.

## Usage
1. **Run `Code.ipybn`**: Open the Jupyter notebook to see the experiments and obtain results.
2. **Review `Report.pdf`**: For an in-depth understanding of the project's methods and outcomes.
