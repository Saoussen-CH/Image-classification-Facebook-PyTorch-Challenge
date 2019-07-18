# Image-classification-Facebook-PyTorch-Challenge

Framework and Libraries : PyTorch, Numpy
Visualisation Libraries : matplotlib, seaborn
Platform : Google Colaboratory GPU

Phases : 

- Data Exploration and preparation :

 - 102 Categories of Flowers Dataset : Unbalanced Dataset
 - Training Dataset : 6552 images
 - Validation Dataset : 817 images
 - Test Dataset : 818 images

+ Techniques : 
 ++ Data Augmentation
 ++ Implementation of a Weighted balancing Sampler

- Modeling and validation Phase : 

+ Techniques : 
 ++ Transfer Learning : Used a Pretained ResNet 200 network architecture trained on ImageNet dataset.
 ++ Replacing ResNet200 classifier with a re-implementation of the Adaptive-average-maxpooling classifier proposed by faster.ai
 ++ Implementation of a training and validation methods
 ++ Used Cross-validation technique
 ++ Fine-tuning the model by unfreezing some feature extraction layers weights and retraining for 
more epochs with new learning rate.

- Testing Phase:

 ++ Implementation of a prediction function
 ++ Testing the trained model on the unseen test dataset resulted on a :
    ** ** Top_1 accuracy : 99,87 % 
     ** ** Top_5 accuracy : 100 %
 ++ Visualization of top_5 class predictions of a new flower image
