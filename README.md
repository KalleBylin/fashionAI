## Introduction & Domain

**Tianchi FashionAI Global Challenge 2018**

According to official statistics from different countries, the market value of the global apparel market is worth over USD 3 trillion. Although artificial intelligence (AI) technology has been evolving along with the fashion industry, there are still different challenges in different areas that need to be addressed.

The analysis of apparel with computers could be easily affected by the dimension and shape of the apparel, distance and angle of shooting, or even how the apparel is displayed or the model is posing. For this reason Tianchi launched a competition with a objective of localizing keypoints on apparel images. This task can help to improve the performance of applications such as alignment, recognition of the local attributes and auto-editing of the images of apparel.

A task like this raises a series of additional challenges. First of all, the dataset consists of 5 different clothing categories: blouse, dress, outwear, skirt and trousers. Each category has different relevant keypoints which adds to the complexity of the model.

Another relevant challenge is dealing with a large amount of images in memory. The neural networks in this notebook are built with Keras, which is a high-level neural networks API written in Python and capable of running on top of TensorFlow, CNTK, or Theano. At the moment of writing, Keras has a built-in generator which works very well on classification tasks but doesn't directly support regression models. 

The idea of this notebook is to explore some of the ways we can deal with these challenges.

## Data

All images are from the Alibaba e-Commerce platform and are more than 54.000 images in total. Most of the images are 512x512 pixels although the size varies slightly throughout the dataset.

This specific dataset concentrates on the keypoint localization of women apparel. There are in total six subsets according to the following six clothes categories: blouse, outwear, trousers, skirt, dress and jumpsuit, respectively. But the organizers decided to omit the jumpsuit since it is uncommon in the real-world scenario. 
