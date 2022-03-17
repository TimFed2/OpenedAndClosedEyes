# OpenedAndClosedEyes
Given a set of 4,000 greyscale low-resolution pictures of open and closed eyes. The goal is to build a classification model

## Model architecture
After varying different models and parameters, I used pre-trained ResNet18 model with the following parameters: 
- Batchsize = 8
- Optimizer - Adam(amsgrad = True, lr = 1.0e-4)
- Schedular - StepLR(gamma = 0.1)

For such specific data only RandomHorizontalFlip was used as an augmentation method. 
Results: 0.9430 accuracy on validation data, 0.97 accuracy on train data
