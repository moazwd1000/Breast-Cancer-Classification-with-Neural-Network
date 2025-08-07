# 🧠 Breast Cancer Detection using Neural Network

This project demonstrates how to detect breast cancer using a simple feedforward neural network built with TensorFlow/Keras. The model is trained on a dataset with 30 features to classify tumors as **benign** or **malignant**.

---

## 📚 Dataset

The dataset used contains numeric features computed from digitized images of breast mass (e.g., mean radius, texture, perimeter, area, etc.).

- **Input features**: 30
- **Target classes**: 2 (Benign, Malignant)
- **Shape**: (samples, 30)

---

## 🏗️ Model Architecture

The model is a simple 3-layer neural network:

| Layer Type | Units | Activation |
|------------|-------|------------|
| Flatten    | 30    | –          |
| Dense      | 20    | ReLU       |
| Dense      | 2     | Softmax    |

### Model Summary:
```plaintext
Input: (30,)
→ Flatten (30 units)
→ Dense (20 units, activation='relu')
→ Dense (2 units, activation='softmax')

✅ Conclusion
The model reaches over 96% training accuracy and 95% validation accuracy after 10 epochs.

It performs well on the validation set, showing no significant overfitting.

This demonstrates that even a simple neural network can effectively classify breast cancer using structured numeric data.
