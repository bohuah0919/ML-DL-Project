Data Source: https://www.kaggle.com/competitions/humpback-whale-identification/data

Description: Using given images of humpback whales to build models to identify individuals of humpback whales.

Notebooks:
- humpbakc-whale1: I implemented ResNet architecture for being familar with it.
- humpbakc-whale2: I used transfer learning to speed up convergence.
- humpbakc-whale3: I used ArcFace loss function to improve performance.

My Best Solution:

Classification:
Models: ResNet34
Image size: 384*384
Augmentation: HorizontalFlip, VerticalFlip, Rotation, GaussianBlur, and Perspective
Loss funtion: ArcFace

Result: Even though my result is better than half historical solution, the result is far from the top solution![my best result](https://user-images.githubusercontent.com/98621364/207476013-b67f29ce-d18e-4d3d-8aa7-0894e30bff8b.png)
