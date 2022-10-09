# Implementing Different Data Augmentation Methods and Explorary Data Analysis on ImageNet

In this notebook, first of all, we show the structure of the ImageNet dataset. Afterward, I did a simple EDA on that. In the next part of this report, I implement several data augmentation methods from ones that are introduced in the class to new methods. Finaly, I evaluate three models: Baseline model which is ResNet-50, ResNet-50 + MixUp, and ResNet-50 + CutMix. We can see the performance of the model with ResNet-50 + CutMix is better than other models.

* EDA - ImageNet
* Data Augmentation
    * 1) Altering the intensities of the RGB channels
    * 2) Image translations (random crops) and horizontal reflection
    * 3) DeepAugmentation
    * 4) CutMix
    * 5) MixUp
* Evaluation of Baseline, MixUp, and CutMix:
    * Because training on ImageNet takes a lots of time, I used pre-trained models.
    
Model | Top-1 Error | Top-5 Error
--- | --- | ---
ResNet-50 (Baseline) | 23.676 | 7.05
ResNet-50 + MixUp | 22.528 | 6.4
**ResNet-50 + CutMix** | **21.4** | **5.924**
