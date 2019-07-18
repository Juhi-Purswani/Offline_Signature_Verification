# Offline_Signature_Verification
Signature samples are classified as forged or genuine using Convolutional Neural Networks.
## Models Used
1. Basic CNN model: **cnn_model.ipynb** contains training for two cnn models. Model 1 contains 2 Convolution Layers, 2 Pooling layers and 2 Dense layers. In the training it was observed that model begins to overfit in epoch 10-20. This can be interpreted with the increment in validation loss. Hence model 2 was implemented by adding 2 Dropout Layers and decrmenting the number of neurons in Dense layers. The results obtained shows that overfitting reduced.
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
| CNN model 2 | 76.54% | 67.77% |
| VGG16 model | 99.72% | 88.02% |

