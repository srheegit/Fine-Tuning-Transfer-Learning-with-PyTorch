# Fine Tuning / Transfer Learning with PyTorch
We build a binary classification model using Fine Tuning / Transfer Learning through PyTorch. We import the model `resnet18` from PyTorch and build two Convolutional Neural Network models, one that is fine-tuned and one that trains only the modified final output layer.

Training a neural network often involves a huge amount of data as well as extensive computational resources. Training a neural network can take days or weeks, and sometime it's not possible for someone with limited data or with limited computational resources to make a machine learning model from scratch that has desirable accuracy. Transfer Learning is one way of dealing with this problem.

Transfer learning is the use of model structures and/or parameters that others have trained on their data for our own machine learning project. In transfer learning, one adopts a model that others have trained, make some modifications on one or more of the layers to be suitable for our own needs, and either (1) fine-tune the model, i.e. start out with the pretrained parameters as initial weights and retrain the whole model, or (2) freeze some layers of the adopted model and (re)train only a portion of the model.

One example of transfer learning is using ChatGPT, or any other Large Language Model (LLM), for specific tasks within a company. Another example of transfer learning is using an image classifier to classify only a few hundreds of personal images.

In this notebook, we shall use PyTorch to come up with a convolutional neural network via transfer learning.

In the end, we are able to achieve an accuracy of around 94% with only 6 epochs, demonstrating the usefulness of transfer learning.
