
# Blood Cell Cancer Classification

## Problem Statement
The goal of this project is to develop a deep learning model that can classify different types of blood cell cancer. The dataset used for this project contains images of blood cell samples belonging to four categories: Benign, Malignant Early Pre-B, Malignant Pre-B, and Malignant Pro-B.

## Dataset
The dataset for this project can be found on Kaggle at the following link:
[Blood Cell Cancer Dataset on Kaggle](https://www.kaggle.com/datasets/mohammadamireshraghi/blood-cell-cancer-all-4class)

The dataset contains the following categories:
- Benign
- Malignant Early Pre-B
- Malignant Pre-B
- Malignant Pro-B

## Data Splitting
The initial dataset consists of a total of 3,242 images. To train and evaluate the model effectively, the dataset was divided into three sets as follows:
- Training Set: 80% of the data (2,592 images)
- Testing Set: 10% of the data (322 images)
- Validation Set: 10% of the data (328 images)

Each set contains images from the four aforementioned categories.

## Data Visualization
Images from both the training and testing sets were visualized to gain a better understanding of the data and its characteristics.

## Model Training Configurations
- Batch Size: 32
- Input Image Size: 224x224 pixels
- Number of Epochs: 5
- Optimizer: Adam

## Model 1: VGG19
The first model used was VGG19, followed by three dense layers, each with 512 neurons. The final output layer was used for classification. The model was compiled and trained for 5 epochs, achieving the following accuracies:
- Training accuracy: 94.3%
- Testing accuracy: 96.5%

## Validation Using the Validation Set
The model's performance was validated using the validation set, which had not been seen by the model. The VGG19 model achieved an accuracy of 95.7% on the validation set.

## Model 2: MobileNetV2
A second model was created using MobileNetV2 as the base model, with the addition of a dense layer containing 512 neurons and the output layer for classification. This new model was compiled and trained for 5 epochs, achieving the following accuracies:
- Training accuracy: 97.5%
- Testing accuracy: 98%

## Improved Validation and Model Saving
The final validation was conducted using the validation set, with the MobileNetV2 model achieving an impressive accuracy of 98.5%. The models were saved using the h5 format to preserve their trained weights and architecture.

## Usage and Necessity
The trained models can play a crucial role in the early detection and prevention of blood cell cancers. Automated classification of blood cell samples can assist medical professionals in making faster and more accurate diagnoses, ultimately improving patient outcomes.

## License
This dataset is provided for educational and research purposes. Please check the original data source for any specific licensing or usage terms.

## Prerequisites
Make sure to install the required Python libraries before running the code. You can use pip to install the necessary packages:

```
pip install tensorflow matplotlib numpy pillow scikit-learn
```

Remember to also download and place the dataset in the appropriate directory as specified in the code.

---
