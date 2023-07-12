# Image_classification-dog_vs_cat
This repository contains two models for classifying dog and cat images:

### CNN Model

The CNN model is built from scratch using TensorFlow. It consists of multiple convolutional layers followed by max pooling, flattening, and fully connected layers. The model is trained on a dataset containing labeled images of dogs and cats.

### Transfer Learning Model with MobileNetV2

The transfer learning model utilizes the pre-trained MobileNetV2 architecture, which has been trained on a large dataset (ImageNet) to classify a wide variety of objects. We fine-tune this pre-trained model to classify dogs and cats.


## Dataset

Both models use the same dataset, which consists of labeled images of dogs and cats. This dataset include 12500 dogs and 12500 cats images, we use 10000 for training and 2500 for testing our model from each of them.
The dataset can be downloaded from the following Kaggle <u>[link](https://www.kaggle.com/datasets/salader/dogs-vs-cats)</u>.

or you can run this command:   
  `**!kaggle datasets download -d salader/dogs-vs-cats**`

`Unzip the dataset using the following code:`
  `import zipfile`
  `zip_ref = zipfile.ZipFile('dogs-vs-cats.zip', 'r')`
  `zip_ref.extractall('dataset')`
  `zip_ref.close()`

  
## Results

The performance of each model can be observed through the training and validation accuracy and loss plots generated during the training process. These plots can help assess the model's learning progress and potential overfitting.
Please refer to the specific model's section above to find the corresponding training and validation plots.

The validation accuracy of CNN model is around: 85%

The validation accuracy of mobilenet_v2 model is around: 97%
