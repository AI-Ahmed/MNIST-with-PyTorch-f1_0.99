<h1 style='background:DarkSlateBlue;
          border-radius: 25px;
          padding: 20px;
          color:white;
          font-size:21px;
          border: 2px solid Lavender;
          font-family:cursive;
          text-align:center'><b>MNIST 🔢 – Getting with start image preprocessing & CV with PyTorch <img width="15" height="20" src='https://i.imgur.com/IvbSjzm.png'/></b></h1>

<center>
    <img src='https://i.imgur.com/fgb7eXs.jpeg'>
</center>

Copyright [2022] [AI Engineer: [Ahmed](https://www.kaggle.com/dsxavier/)]

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

# 📖<font size='5' color='DarkViolet'>Overview</font>

MNIST ("Modified National Institute of Standards and Technology") is the de facto “hello world” dataset of computer vision. Since its release in 1999, this classic dataset of handwritten images has served as the basis for benchmarking classification algorithms. As new machine learning techniques emerge, MNIST remains a reliable resource for researchers and learners alike.

In this competition, your goal is to correctly identify digits from a dataset of tens of thousands of handwritten images. We’ve curated a set of tutorial-style kernels which cover everything from regression to neural networks. We encourage you to experiment with different algorithms to learn first-hand what works well and how techniques compare.

# 📝<font size='5' color='DarkViolet'>Acknowledgments</font>

More details about the dataset, including algorithms that have been tried on it and their levels of success, can be found at http://yann.lecun.com/exdb/mnist/index.html. The dataset is made available under a Creative Commons Attribution-Share Alike 3.0 license.

# 📝<font size='5' color='DarkViolet'>Proof of Work</font>

**MNIST** considers being the first case study the scientists start doing their experiments on it during the 70s, and now it is one of the essential datasets that most scientists are using to verify their networks. 

If you want to start exploring the field of image processing and computer vision **(CV)**, you start from the right place. 

It is not just working on code more than exploring the field with you, guys. I would like to put what I have learnt into this kernel step by step so that we can come up with something simple and efficient to show you how beautiful this field is and how it can help you in further industries. Thank you for following up with my work!

# 📚<font size='5' color='DarkViolet'>Data Dictionary</font>

The data files `train.csv` and `test.csv` contain **gray-scale images of hand-drawn digits**, <u>from zero through nine</u>.

Each image is **28 pixels in height and 28 pixels** in width, for a total of **784 pixels** in total. Each pixel has a single pixel-value associated with it, indicating the lightness or darkness of that pixel, with higher numbers meaning darker. This pixel-value is an integer between <u>0 and 255, inclusive</u>.

The training data set, (train.csv), has 785 columns. The first column, called "label", is the digit that was drawn by the user. The rest of the columns contain the pixel-values of the associated image.

Each pixel column in the training set has a name like pixelx, where x is an integer between 0 and 783, inclusive. To locate this pixel on the image, suppose that we have decomposed x as x = i * 28 + j, where i and j are integers between 0 and 27, inclusive. Then pixelx is located on row i and column j of a 28 x 28 matrix, (indexing by zero).

For example, pixel31 indicates the pixel that is in the fourth column from the left, and the second row from the top, as in the ascii-diagram below.

Visually, if we omit the "pixel" prefix, the pixels make up the image like this:

```markdown
000 001 002 003 ... 026 027
028 029 030 031 ... 054 055
056 057 058 059 ... 082 083
 |   |   |   |  ...  |   |
728 729 730 731 ... 754 755
756 757 758 759 ... 782 783 
```

The test data set, (test.csv), is the same as the training set, except that it does not contain the "label" column.

Your submission file should be in the following format: For each of the 28000 images in the test set, output a single line containing the ImageId and the digit you predict. For example, if you predict that the first image is of a 3, the second image is of a 7, and the third image is of a 8, then your submission file would look like:

```markdown
ImageId,Label
1,3
2,7
3,8 
(27997 more lines)
```
