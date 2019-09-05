`Status: In Progress`
## Unconventional Neural Networks
> __For the unfamiliar:__ Generative models are one of the most promising approaches towards this goal. To train a generative model we first collect a large amount of data in some domain (e.g., think millions of images, sentences, or sounds, etc.) and then train a model to generate data like it. The intuition behind this approach follows a famous quote from Richard Feynman:

###### “What I cannot create, I do not understand.” — Richard Feynman
    
> The trick is that the neural networks we use as generative models have a number of parameters significantly smaller than the amount of data we train them on, so the models are forced to discover and efficiently internalize the essence of the data in order to generate it.

![Deep Dream](https://i0.wp.com/www.ideatovalue.com/wp-content/uploads/2016/07/deep-dreams.jpg?ssl=1)

### Objective
> This repository is dedicated to playing around with neural networks. The idea here is to poke around with various neural networks, doing unconventional things with them. Doing things like trying to teach a sequence to sequence model math, doing classification with a generative model, and so on. I've wanted to do this, but haven't thought of a way to compile them, this will have to do!

![Deep Dream 2](https://i.ytimg.com/vi/DgPaCWJL7XI/maxresdefault.jpg)
##### References
> My main focus is on implementing various kinds of Generative Adversarial Networks and Variational AutoEncoders and special thanks to [sentdex](https://pythonprogramming.net/generative-model-python-playing-neural-network-tensorflow/), [kaggle](https://www.kaggle.com/c/generative-dog-images) and [eriklindernoren](https://github.com/eriklindernoren/Keras-GAN) for making this repository a combination of amazing generative models.  

__A foundation of Machine Learning and Deep Learning with TensorFlow specifically is necessary for understanding.__

### Dependencies
At the very least, right now, you will need TensorFlow installed, and Python of course! I am currently using:

    * Python 3.6

    * TensorFlow 2.0 / Tensorflow 1.7

<!-- If you want to follow along on the CPU, you may have trouble with long training times, but you can still do it with a pip install --upgrade tensorflow or pip install -U --pre tensorflow to get the latest version of Tensorflow. If you plan to follow along with TensorFlow on the GPU, then you will also need the to install the Cuda Toolkit and the matching CuDNN. See the TensorFlow install page for which version of CuDNN and the Cuda Toolkit you need. For installing the GPU version of TensorFlow, you can see my TensorFlow-GPU Windows installation tutorial or the Linux Tensorflow-GPU setup tutorial, both of which are with older version of TensorFlow, but the steps are the same (Get TF, CUDA Toolkit, and copy over the CuDNN files).-->

<p align="center">
  <img src="https://camo.githubusercontent.com/15ad5010011227a7ab8c6c77d19b7cc625cced30/687474703a2f2f6572696b6c696e6465726e6f72656e2e73652f696d616765732f67616e5f6d6e697374352e676966">
</p>

### The World of Generative Model
> I've personally always really liked generative models. They are relatively quick to train, requiring very little data, but can produce results very similar to the input you fed them. They don't appear to have much practical use as of yet, but you can do fun things with them, like making art, making music and such.

#### **What's known as a Character-Level Generative Neural Network.?** 
> The "character" part of this just means it'll generate new sequences by using individual characters. In most cases, this is for language like tasks, but this doesn't HAVE to be the case. Let's first check it out with a real language, however. The most simple-to-use implementation that I've seen for a character-level generative model in TensorFlow is the char-rnn-tensorflow project on GitHub from Sherjil Ozair. Just in case things have changed and you want to follow along exactly, the exact commit I am working with is: 401ebfd Go ahead and Grab/clone this package, extract if necessary, and let's see what we've got here.
