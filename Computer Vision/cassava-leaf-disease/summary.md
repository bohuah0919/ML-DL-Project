Data Source: https://www.kaggle.com/competitions/cassava-leaf-disease-classification/data

Description: Using given images of cassava leaves to build models to classify the type of diseases.

Solution:

Classification:
- Models: ResNext34
- Image size: 448*448
- Augmentation: RandomResizedCrop, HorizontalFlip, VerticalFlip, and ShiftScaleRotate
- Loss function: Cross Entropy with label smoothing

Useful Idea:
Label smoothing

Result: I finally get a score 0.886 for this project, it is close to most scores from historical competition participants!

![QQ图片20221212181315](https://user-images.githubusercontent.com/98621364/207478740-400570a2-2af3-418f-9734-ea2c574cb101.png)
