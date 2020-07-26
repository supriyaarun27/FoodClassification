# Food Classification

### Problem : Classification of food images from the FOOD 101 dataset 


### What is transfer Learning ? 


I have used transfer learning on a pretrained Resnet50 model that has been pre-trained on the ImageNet Dataset. Fast.ai, provides the vision.learner module to easily implement transfer learning. Transfer learning uses pre-trained models to solve new problems. In this method, pre-trained models can be retrained with some layers frozen. This improves the model's ability to learn specific areas where the basic underlying information is already learnt as it is pre-trained. 


More information on Fast.ai's transfer learning module here : 
https://docs.fast.ai/vision.learner.html

### Why did I pick ResNet50 ? 

This neural network architecture as suggested by the name has 50 layers. A common problem with other existing architectures like ImageNet, AlexNet etc, was that the deeper the model was harder it got to train these models. Deeper models are on a trend as it helps in making sure that the data is not overfitting. But, deeper models also come with the issue of vanishing gradients. As the gradient is multiplied through the layers in back propogation -- repeated multiplication can lead to small and vanishing gradients. Hence the performance of the "deep" neural net starts to diminish. ResNet introduced the "skip connections" that would skip one or more layers. 


### Why is an optimum learning rate important?

Learning rate is an hyperparameter that is used to tune the model is response to the error estimated everytime the model weights are changed. Choosing the learning rate is challenging as a value too small may result in a long training process that could get stuck, whereas a value too large may result in learning a sub-optimal set of weights too fast or an unstable training process.

Fast.ai has an LR finder that is quite handy in finding the optimal learning rate. More on this here : https://docs.fast.ai/basic_train.html




