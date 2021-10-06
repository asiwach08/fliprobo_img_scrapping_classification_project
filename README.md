
##  Amazon Image Classification Project Using Neural Networks

![](https://cdn.analyticsvidhya.com/wp-content/uploads/2020/02/ANN-Graph.gif)
  


Images are one of the major sources of data in the field of data science and AI. This field is making appropriate use of information that can be gathered through images by examining its features and details. We are trying to give  an exposure of how an end to end project is developed in this field. 
The idea behind this project is to build a deep learning-based Image Classification model on images that will be scraped from e-commerce portal. This is done to make the model more and more robust.




## Acknowledgements

 - [stackoverflow](https://stackoverflow.com/)
 - Notes and Repositry from DataTrained
 - FlipRobo Technologies
 - [ML Algorithms from analyticsvidhya](https://www.analyticsvidhya.com/blog/2017/09/common-machine-learning-algorithms/)

## Motivation

In today world we are dealing with lots of data which is present in various formats like numbers ,categories, images etc. The data present in numbers or categorical form is easy to store and understand but image data is somehow different form these. In image data we have to use some different techniques to deal it and these new techniques and way to deal image data motivates me to undertake this project and build a model for image classification.
## Libraries Required


- [Numpy](https://numpy.org/doc/stable/)
- [Matplotlib](https://matplotlib.org/stable/contents.html)
- [Tensorflow](https://www.tensorflow.org/api_docs/python/tf)
- [Keras](https://keras.io/api/)
- [Selenium](https://www.selenium.dev/documentation/)
- [time](https://docs.python.org/3/library/time.html)
  
## Installation

The Code is written in Python 3.9. If you don't have Python installed you can find it here. If you are using a lower version of Python you can upgrade using the pip package, ensuring you have the latest version of pip. To install the required packages and libraries, run this command in the project directory:

```bash
  npip install -r requirements.txt

```
    
## Technical Aspects

This is a Deep Learning project  and divided into 2 phases -

1.  Data Collection Phase :
            In this section, we scraped images from e-commerce portal, Amazon.com. The clothing categories used for scraping was:
   -	Sarees (women)
   -	Trousers (men)
   -	Jeans (men)
2. Model Building Phase: 
          After the data collection and preparation is done, we have to build an image classification model that will classify between these 3 categories mentioned above. 

## Training Accuracy with Epochs
![](data:image/png;base64,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%0A)
## 🚀 About Me
I'm a Data Analyst/Data Science intern at FlipRobo Technologies trying to enhance my skills and knowledge.

  
## 🔗 Links
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/asheem-siwach-a52987152/)

  
## 🛠 Skills

Python, Stastistics, DL...

  
