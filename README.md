# 🧠 Deep Learning Assignment: MNIST Classification with Multiple Optimizers & Activations

This project implements a fully-connected neural network **from scratch using NumPy** for classifying handwritten digits from the **MNIST** dataset. The network is trained using various **activation functions** and **optimizers**, allowing a comparative analysis of their impact on performance.

## 📌 Features

* ✅ Manual implementation of neural networks (no TensorFlow/PyTorch)
* ✅ Supports multiple **activation functions**: `ReLU`, `Sigmoid`, `Tanh`, `Leaky ReLU`
* ✅ Includes popular **optimizers**: `SGD`, `Mini-Batch SGD`, `Momentum`, `Adam`, `Adagrad`, `Adadelta`
* ✅ Visual comparison of accuracy trends
* ✅ Evaluation on **MNIST** dataset (70k grayscale images)

---

## 📊 Activation Functions & Optimizers Compared

| Activation Function | Optimizers Tested                                    |
| ------------------- | ---------------------------------------------------- |
| ReLU                | SGD, MiniBatchSGD, Momentum, Adam, Adagrad, Adadelta |
| Sigmoid             | SGD, MiniBatchSGD, Momentum, Adam, Adagrad, Adadelta |
| Tanh                | SGD, MiniBatchSGD, Momentum, Adam, Adagrad, Adadelta |
| Leaky ReLU          | SGD, MiniBatchSGD, Momentum, Adam, Adagrad, Adadelta |

Each combination is evaluated over 10 epochs using a network with the architecture:

```
Input Layer (784) → Hidden Layer 1 (128) → Hidden Layer 2 (64) → Output Layer (10)
```

---

## 📈 Visual Results

Two sets of plots are generated:

1. **Optimizers Comparison (for each Activation)**
2. **Activations Comparison (for each Optimizer)**

These allow you to observe the effect of optimizers and activation functions independently.

---

## 🧪 Final Test Accuracy

| Activation + Optimizer                          | Accuracy |
| ----------------------------------------------- | -------- |
| ReLU + Adam                                     | \~0.97 ✅ |
| Tanh + Adam                                     | \~0.96   |
| Leaky ReLU + Adam                               | \~0.965  |
| Sigmoid + SGD                                   | \~0.92   |


---

## 🧬 Project Structure

```
├── neural_network.py        # Main NN architecture and training logic
├── activations.py           # Activation functions and their derivatives
├── optimizers.py            # SGD, Adam, Adagrad, Adadelta, etc.
├── run_experiments.py       # Training loop for all combinations
├── visualizations.py        # Accuracy plots
└── README.md                # Project overview
```

---

## ⚙️ Requirements

Install the required Python packages:

```bash
pip install numpy matplotlib scikit-learn
```

---

## 🚀 How to Run

```bash
python run_experiments.py
```

This script:

* Trains 24 combinations (4 activations × 6 optimizers)
* Stores and plots training accuracy over epochs
* Prints test set accuracy for each trained model

---

## 🧠 What You Learn

* How activation functions affect gradient flow and learning
* How different optimizers influence convergence
* How to implement a neural network from scratch (forward + backward pass)
* Practical deep learning experimentation without relying on high-level libraries

---

## 📚 Dataset Used

* [MNIST Handwritten Digits](https://www.openml.org/d/554)
* 70,000 grayscale 28×28 images (10 classes: 0–9)

---

## 📌 Future Improvements

* Add dropout & batch normalization
* Add model saving/loading
* Add learning rate scheduler
* Extend to other datasets (e.g., Fashion-MNIST)

---

## 🧑‍💻 Author

**Swapnil Halder**
🔗 [LinkedIn](https://www.linkedin.com/in/swapnilhalder/)

---

> ⭐ Star this repository if it helped you learn or if you like the clean from-scratch implementation!

---

