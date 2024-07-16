# Text-Generation-with-PyTorch-Techniques-and-Examples
Welcome to the "Text Generation with PyTorch" repository! This repository is dedicated to showcasing various techniques and examples of text generation using PyTorch.

# Bigram Language Model
![bigram img](https://github.com/faezeh-gholamrezaie/Text-Generation-with-PyTorch-Techniques-and-Examples/blob/main/image/Image-bigram.png)

The bigram model is used to generate characters. We train the model using a notebook written by a wizard as the dataset, which consists of 81 unique characters. Each character is represented as a (1 * 1) vector. Since there are 81 characters and each batch has 4 blocks, with each block containing 8 characters, the input dimension for the model is (4 * 8 * 81) after applying the nn.Embedding. After reshaping the tensor, the dimension becomes (32 * 81). In other words, the reshaped vector represents 32 characters, and we use it to predict the next most probable character.

# Resources:

wizard_of_oz.txt : https://github.com/kwartler/text_mining/tree/master
