# Object Classification

[Image Classification](https://en.wikipedia.org/wiki/Computer_vision#Recognition) (or Image Identification) is one of the pilot use cases for deep learning. The goal of the task is to train a model capable of identifying the main object of interest in an image. *What can you use it for?* Here are a few ideas - [identify landmarks in photos](https://ai.googleblog.com/2018/03/google-landmarks-new-dataset-and.html), [ImageNet challenge](http://www.image-net.org/challenges/LSVRC/), identifying celebrities (or yourself) in images, detecting anomalies in medical images.

### Try it now

[![Run on FloydHub](https://static.floydhub.com/button/button.svg)](https://floydhub.com/run?template=https://github.com/floydhub/image-classification-template)

Click this button to open a Workspace on FloydHub that will train this model.

### Dog Breed Classification

In this notebook, we will build a model to identify dog breeds in an image. How well you can tell your Norfolk Terriers from your Norwich Terriers? 

[Classification](https://raw.githubusercontent.com/floydhub/image-classification-template/master/images/classification.png)

We will use the [Kaggle's Dog Breed Dataset](https://www.kaggle.com/c/dog-breed-identification) dataset for training. With 120 breeds of dogs and a limited number training images per class, you might find the problem more, err, ruff than you anticipated. 

To speed things up, we will apply [Transfer Learning](https://cs231n.github.io/transfer-learning/) by [building new layers on top of the Xception model]( https://www.depends-on-the-definition.com/transfer-learning-for-dog-breed-identification/mode) pre-trained on ImageNet to classify the top 10 dog breeds. *Note: We have reduced the number of classes (i.e. dog breeds) to 10 to fit the model in a CPU machine.*

We will:
- Preprocess images data for computer vision tasks
- Transfer Learning: build new layers on top of the pretrained Xception model using Keras and Tensorflow
- Evaluate our model on the test set
- Run the model on new dog images from the web!
