# Early Alzheimer’s Detection Using Deep Learning with ResNet152V2 on MRI Images

## Overview

This project focuses on the early detection of Alzheimer’s disease using deep learning techniques. By leveraging the ResNet152V2 architecture, the model is trained to classify different stages of Alzheimer’s disease from Magnetic Resonance Imaging (MRI) scans. Early detection can aid in timely treatment and care for patients, potentially improving their quality of life.

## Objectives

1. Develop a robust machine learning model using transfer learning with the ResNet152V2 architecture.
2. Quantitatively evaluate the model's accuracy in detecting and classifying Alzheimer’s stages based on MRI images.

## Dataset
- Dataset used in this project provided by Kaggle user [Uraninjo](https://www.kaggle.com/uraninjo)
- Link to Dataset : [Augmented Alzheimer MRI Dataset V2](https://www.kaggle.com/datasets/uraninjo/augmented-alzheimer-mri-dataset-v2)

## Methodology

- **Data Preprocessing**: MRI images are resized to 224x224 pixels and rescaled to a range of 0-1.
- **Model Architecture**: The model is built using the ResNet152V2 pre-trained on ImageNet for transfer learning.
- **Training and Validation**:
  - Dataset split: Training (70%), Validation (20%), Testing (10%).
  - Applied techniques like data augmentation and dropout layers to reduce overfitting.
- **Evaluation Metrics**: Accuracy, precision, recall, and F1 score are used to assess model performance.

## Built With

- **Python** - Programming language used for development
- **TensorFlow** - Deep learning framework for building the model
- **NumPy** - Library for numerical computations
- **Matplotlib** - Library for data visualization
- **Scikit-learn** - Tools for model evaluation and metrics
- **Google Colab** - Cloud-based platform for running Jupyter notebooks

## Source Code

The implementation details are available in the repository. Refer to the following file for functionality:

- [`AD_New_Model.ipynb`](./AD_New_Model.ipynb): Script to train and test the ResNet152V2 model on MRI data.

## Results

- Achieved a classification accuracy of 97% on the test dataset.
- Precision, recall, and F1 score for each class are as follows:

| Class    | Precision | Recall | F1 Score |
| -------- | --------- | ------ | -------- |
| Non Demented   | 96%       | 99%    | 98%      |
| Very Mild Demented     | 98%       | 95%    | 96%      |
| Mild Demented | 100%       | 95%    | 98%      |
| Moderate Demented   | 100%       | 100%    | 100%      |

## Future Work

1. Explore other deep learning architectures like EfficientNet or Vision Transformers.
2. Increase dataset size for better generalization.
3. Implement explainable AI (XAI) techniques to visualize decision-making.

## Acknowledgments

This project was inspired by the need to assist in early detection of Alzheimer’s disease using computational physics and machine learning techniques.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

*All rights reserved by Rui Costa Raka Milanisti. Inspired by experiences from Bangkit Academy and computational physics studies.*

