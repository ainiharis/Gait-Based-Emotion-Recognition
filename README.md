# Gait Based Emotion Recognition Using Pre-Trained Model
Using pre-trained deep learning models to recognize emotions based on how people walk. By adapting models trained on large datasets, the goal is to apply this to real-world situations, such as monitoring emotions in the elderly or improving virtual experiences.

## Dataset
https://drive.google.com/drive/folders/1YgHBwrOJUrOjy4YgpnopE2Rg7QAjPoEC?usp=sharing

## Summary of optimal hyperparameters for the Gait-Densenet121
| Hyperparameters       | Tested Values                             | Optimal Value |
|-----------------------|---------------------------------------------|---------------|
| Input Size            | 128×128, 224×224                           | 224×224       |
| Batch Size            | 32, 64, 128                                 | 32            |
| Optimizer             | Adam, Nadam, SGD                            | Adam          |
| Learning Rate         | 0.01, 0.001, 0.0001, 0.00001               | 0.0001        |
| Activation Function   | ReLU, LeakyReLU                             | ReLU          |
| Dropout Layer         | 0.3, 0.4, 0.5, 0.6                          | 0.3           |
| **Accuracy**          | —                                           | **99.74%**    |

