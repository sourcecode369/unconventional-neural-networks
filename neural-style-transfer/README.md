## Neural Style Transfer

> Neural style transfer is an optimization technique used to take two images—a content image and a style reference image 
(such as an artwork by a famous painter)—and blend them together so the output image looks like the content image, 
but “painted” in the style of the style reference image.

#### This is implemented by optimizing the output image to match the content statistics of the content image and the style 
#### statistics of the style reference image. These statistics are extracted from the images using a convolutional network.

#### For example, let’s take an image of this dog and Wassily Kandinsky's Composition 7:

![content_image](https://storage.googleapis.com/download.tensorflow.org/example_images/YellowLabradorLooking_new.jpg)

![style_image](https://storage.googleapis.com/download.tensorflow.org/example_images/Vassily_Kandinsky%2C_1913_-_Composition_7.jpg)

#### Now how would it look like if Kandinsky decided to paint the picture of this Dog exclusively with this style? Something like this?

![style_transfer](https://tensorflow.org/tutorials/generative/images/stylized-image.png)
