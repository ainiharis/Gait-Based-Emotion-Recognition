## Gait Based Emotion Recognition Using Pre-Trained Model
Using pre-trained deep learning models to recognize emotions based on how people walk. By adapting models trained on large datasets, the goal is to apply this to real-world situations, such as monitoring emotions in the elderly or improving virtual experiences.


### E-Walk Dataset
https://drive.google.com/drive/folders/1YgHBwrOJUrOjy4YgpnopE2Rg7QAjPoEC?usp=sharing


### Model Comparison
Between the seven tested models, the goal was to choose one with moderate accuracy (90–95%), providing strong learning ability while still leaving room for improvement. Based on this, InceptionV3 and DenseNet121 were the best candidates.

**DenseNet121** was selected because, although slightly less accurate, it is a modern and efficient architecture with dense layer connections that improve feature reuse and gradient flow.

| Pre-Trained Model | Accuracy (%) | Training Time (s) |
|-------------------|--------------|--------------------|
| VGG16             | 97.37        | 260.43             |
| Xception          | 97.37        | 1206.12            |
| InceptionV3       | 94.21        | 1007.21            |
| ResNet50          | 47.89        | 618.64             |
| MobileNetV2       | 96.84        | 989.55             |
| EfficientNetB0    | 25.00        | 145.59             |
| **DenseNet121**   | **91.58**    | **1126.63**        |


### Summary of optimal hyperparameters for the Gait-Densenet121
Accuracy after enhancement: 99.74%

| Hyperparameters       | Tested Values                             | Optimal Value |
|-----------------------|---------------------------------------------|---------------|
| Input Size            | 128×128, 224×224                           | 224×224       |
| Batch Size            | 32, 64, 128                                 | 32            |
| Optimizer             | Adam, Nadam, SGD                            | Adam          |
| Learning Rate         | 0.01, 0.001, 0.0001, 0.00001               | 0.0001        |
| Activation Function   | ReLU, LeakyReLU                             | ReLU          |
| Dropout Layer         | 0.3, 0.4, 0.5, 0.6                          | 0.3           |
| **Accuracy**          | —                                           | **99.74%**    |

