Data Source: https://www.kaggle.com/competitions/severstal-steel-defect-detection/data

Description: Using given images of defective steels to build models to classify the type of defect, and detect the place of the defect.

Solution:
- Classification: 
  1. Models: the best ResNet34 and top two best efficientnet_b3
  2. Image size: full size
  3. Augmentation: HorizontalFlip, VerticalFlip, and RandomBrightnessContrast
  4. TTA: HorizontalFlip
- Detection: 
  1. Models: top two best Unet with ResNet18 and the best FPN with ResNet50
  2. Image size: full size
  3. Augmentation: HorizontalFlip, VerticalFlip
  4. TTA: HorizontalFlip

Working Ideas:
1. TTA in the classification increases the score by 0.003
2. TTA in detection increases the score by 0.003
3. Dropping small size areas in detection increases the score by 0.002
4. Changing the threshold from 0.5 to 0.6 in classification and detection increases the score by 0.002.

Result:
I finally get a score 0.8882 for this project, it can enter the top 25% of scores from historical competition participants
![steel defect detection result](https://user-images.githubusercontent.com/98621364/207207008-7cc56e48-ad5b-4ada-8193-aafd6aae9191.png)
