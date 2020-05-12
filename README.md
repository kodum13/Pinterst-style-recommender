# Pinterst-style-recommender

This model uses Pinterest boards as input for a neural network model in Keras and recommends new styles for me.

To interact with Pinterest, I used the py3-pinterest library from https://pypi.org/project/py3-pinterest/.
The VGG16 convolutional neural network model is implemented with the help of Keras based on the tutorial "Building Deep Learning Applications with Keras 2.0" by Adam Geitgey to create probabilities that I will like the style. 
https://www.tensorflow.org/api_docs/python/tf/keras/applications/VGG16

Steps to create this project:
1. Set up two Pinterst boards, one with styles you like and the other with styles you don't. 
2. Read in the pins from both boards and add labels such as 0 for those you like and 1 for those you don't. (pinterest_images)
3. Train a neural net using Keras to distinguish between clothing styles to recommend. (model_train)
4. Get new recommendations from Pinterst using py3-pinterest library. (pinterest_recs)
5. From the new pins have the model predict which pins you will like. (model_score)
6. Add those recommended pins to a new board. (model_test)
7. Enjoy styles on Pinterest without having to constantly pin new photos!

![pinterest style](https://github.com/kodum13/Pinterst-style-recommender/blob/master/pinterst_style.png)
