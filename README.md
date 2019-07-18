# Offline_Signature_Verification
Signature samples are classified as forged or genuine using Convolutional Neural Networks.
## Models Used
1. Basic CNN model: **cnn_model.ipynb** contains training for two cnn models. Model1 contains two Convolution Layers, two Pooling layers and two Dense layers. In the training it was observed that model begins to overfit in epoch 10-20. This can be interpreted with the increment in validation loss.<br>
To reduce overfitting model2 was implemented by adding 2 Dropout Layers, decrementing the number of neurons in Dense layers and applying L2 regularization in Dense Layers. The results obtained shows that overfitting reduced and validation loss does not increased.
2. VGG16 model: **vgg16.ipyn** contains implemetation of VGG16 model pretrained on imagenet dataset. In 1st model all the layers were trained. In 2nd model some of the starting layers were freezed and then trained on the data.
Both models are implemented using Tensorflow Keras api.
## Dataset
The dataset used was taken from a hackerearth AI challenge.
This is the link: https://www.hackerearth.com/challenges/hackathon/axis-hackathon/
## Requirenments
* Python 3
* Matplotlib
* Numpy
* Tensorflow
* Keras
## Results
| Model | Training Accuracy | Valiation Accuracy |
| ------ | ---------------- | ------------------ |
| CNN model 1 | 99.44% | 67.77 % |
| CNN model 2 | 84.92%% | 74.38% |
| VGG16 model | 99.72% | 88.02% |

