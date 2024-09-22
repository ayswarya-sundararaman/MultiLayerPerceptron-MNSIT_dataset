
# MLP Assignment - MNIST Dataset

This project implements multi-layer perceptron (MLP) models to classify handwritten digits from the MNIST dataset using Keras. The project explores the impact of adding layers, Batch Normalization (BN), and Dropout on model performance.

## Dataset

- **Dataset**: MNIST (60,000 training images, 10,000 test images)
- **Input Shape**: 784 (flattened 28x28 pixel images)
- **Classes**: 10 (digits 0-9)

## Models Implemented

1. **Model 1: 2-Layer MLP**
   - Without BN and Dropout
   - With BN and Dropout

2. **Model 2: 3-Layer MLP**
   - Without BN and Dropout
   - With BN and Dropout

3. **Model 3: 5-Layer MLP**
   - Without BN and Dropout
   - With BN and Dropout

## Key Observations

- **Batch Normalization** helps in faster convergence and improved accuracy.
- **Dropout** reduces overfitting, improving test performance.
- Models with more layers tend to converge faster in early epochs.
- **Accuracy**: Up to 97% accuracy was achieved with just 2 layers, and adding BN and Dropout further improved results to 98%.

## Results Summary

|  Model  | Layers | Batch Normalization & Dropout | Train Loss | Test Loss | Test Accuracy |
|---------|--------|-------------------------------|------------|-----------|---------------|
| Model 1 |   2    | No                            |    0.01    |    0.09   |      0.97     |
| Model 1 |   2    | Yes                           |    0.07    |    0.07   |      0.98     |
| Model 2 |   3    | No                            |    0.03    |    0.09   |      0.97     |
| Model 2 |   3    | Yes                           |    0.05    |    0.08   |      0.98     |
| Model 3 |   5    | No                            |    0.04    |    0.09   |      0.97     |
| Model 3 |   5    | Yes                           |    0.10    |    0.10   |      0.97     |

## Conclusion

The MLP model with 2 layers, batch normalization, and dropout provides the best accuracy and performance with minimal overfitting.
