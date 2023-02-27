# Fruit Classification

## Problem Statement
Although a fruit recogition system is not necessarily important, it would be beneficial to have one that can classify different types of fruits and vegetables. A customer would click an image with his smart phone and upload it in the application for the store to detect the fruit's name and return it back to the customer.

## Model
I used transfer learning, with the help of the famous EfficientNetB3 model, trained on ImageNet.

![EfficientNetB3](https://user-images.githubusercontent.com/62629426/221706810-2cda4cc9-2b40-45eb-b5eb-f7c518739d61.png)

As we can see that EfficientNet achieves the highest accuracy, whilst having the least parameters out of most modern CNN architectures.

<img width="500" alt="models" src="https://user-images.githubusercontent.com/62629426/221452049-30538255-0bc4-4d62-84c1-19cf5608a84d.png">

EfficientNet are also scaled in a more principled way, than other models, basically, everything is gradually increasing.

![image](https://user-images.githubusercontent.com/62629426/221708947-8fa7e019-6f04-4bfb-a79a-e3e1b93bd681.png)
*(a) is a baseline network example; (b)-(d) are conventional scaling that only increases one dimension of network width, depth, or resolution. (e) is our proposed compound scaling method that uniformly scales all three dimensions with a fixed ratio.*

To get more information about the EfficientNet architecture check this out (https://towardsdatascience.com/complete-architectural-details-of-all-efficientnet-models-5fd5b736142)

### Libraries: 
- [Tensorflow - Keras](https://www.tensorflow.org/api_docs/python/tf/keras)
- [tensorflow](https://www.tensorflow.org/)
- [Numpy](https://numpy.org/)
- [Matplotlib](https://matplotlib.org/)

### Results:
one of 15 fruits
  - apple_braeburn_1
  - apple_golden_1
  - apple_granny_smith_1
  - apple_pink_lady_1
  - apple_red_1
  - apple_red_delicios_1
  - apple_rotten_1
  - cabbage_white_1
  - carrot_1
  - cucumber_1
  - eggplant_violet_1
  - pear_1
  - pear_2
  - zucchini_1
  - zucchini_dark_1 

### Accuracy:
- accuracy: 0.9896 
- Loss: 0.0222
- Val_accuracy: 0.8750
- Val_loss: 0.6089
