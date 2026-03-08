# Neural Network From Scratch for Handwritten Digit Recognition

Built a feedforward neural network from first principles in Python to classify handwritten digits from the MNIST dataset. Starting from a simple 3-layer architecture, I improved test accuracy from **94.26%** to **97.48%** through structured hyperparameter tuning.

## Snapshot

- **Implemented machine learning fundamentals from scratch**: forward propagation, sigmoid activation, error calculation, and backpropagation without TensorFlow or PyTorch
- **Worked with real image data at scale**: trained on **60,000** MNIST examples and evaluated on **10,000** holdout examples
- **Ran measurable experiments**: tuned learning rate, number of training epochs, and hidden-layer size
- **Delivered quantified improvement**: increased accuracy by **3.22 percentage points** and reduced classification error by about **56%**
- **Used core data science tooling**: Python, NumPy, Pandas, SciPy, Matplotlib

## Project Snapshot

| Area | Details |
| --- | --- |
| Problem | Multi-class image classification on handwritten digits |
| Dataset | MNIST (`60,000` training images, `10,000` test images) |
| Model | 3-layer neural network (`784 -> hidden -> 10`) |
| Baseline | `100` hidden nodes, learning rate `0.3`, 1 pass through training data |
| Best Configuration | `700` hidden nodes, learning rate `0.1`, `7` epochs |
| Best Test Accuracy | **97.48%** |

## What I Actually Built

- Loaded and explored raw MNIST CSV data using Pandas
- Visualized 28x28 grayscale digit images with Matplotlib
- Normalized pixel intensities from raw `0-255` values to a stable training range of `0.01-1.00`
- Encoded labels into target vectors for multi-class classification
- Wrote a custom `NeuralNetwork` class using NumPy matrix operations
- Implemented manual weight updates with backpropagation
- Evaluated predictions with a clean train/test workflow
- Compared multiple model configurations and selected the strongest performer based on test accuracy

## Experimental Results

| Experiment | Best Setting | Best Accuracy |
| --- | --- | --- |
| Learning rate sweep | `0.1` | `94.83%` |
| Epoch sweep | `7` epochs | `96.57%` |
| Hidden-layer width sweep | `700` hidden nodes | **97.48%** |

## Data Science Skills Demonstrated

- **Machine learning fundamentals**: neural network architecture, activation functions, gradient-based learning, model evaluation
- **Experimentation**: controlled parameter sweeps, comparison of model performance, evidence-based model selection
- **Data handling**: preprocessing high-dimensional input data, label transformation, train/test separation
- **Programming**: object-oriented Python, vectorized NumPy operations, reproducible notebook workflow
- **Communication**: translated experiments into interpretable plots and concise performance takeaways
