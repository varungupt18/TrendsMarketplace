## Image Analysis with Amazon Rekognition
**Group 15: Chien-Chu Hsu, Pankhuri Tyagi, Samarth Patil, Sarasija Gaddameedi, Varun Gupta, Yutian Sun**



Introducing Amazon Rekognition: Automating Image Analysis With Machine Learning
This project explores how Amazon Rekogntion can be used for image recognition and comparison.

**Challenges in Image analysis:** Using machine learning for image analysis can be quite expensive and time consuming as it requires a lot of processing power. Additionally, image data can be quite unstructured, coming in different formats and sizes. 

We introduce Amazon Rekogntion, an image analysis service available in AWS. This can be leveraged by organizations to analyze and compare images on the go. We will be using the Chest X-Ray Images and the task is to detect which images indicate that the patient has pneumonia. 

**Data Description:**
The data can be found at the following link: 
https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia

There are 5,863 X-Ray images (JPEG) and 2 categories (Pneumonia/Normal).
<br>

**Workflow:**

<br>

![image](https://media.github.umn.edu/user/22682/files/b659afb6-5fc8-4401-ad03-1b65d8a48d33)

<br>
<br>

**Importing Data**: Data can be imported into Rekogntion in the following ways:
<br>

![image](https://media.github.umn.edu/user/22682/files/f8ce4cef-c630-46cd-b671-ea49b4c3c81c)

<br>

**Labeling Images:** The Rekognition Custom Labels console provides a visual interface to make labeling your images fast and simple. The interface allows you to apply a label to the entire image or to identify and label specific objects in images using bounding boxes with a simple click-and-drag interface. Alternatively, Rekognition can automatically assign image-level labels to images based on the folder name. 
This is what we did in our case as we had the data in two folders labeled 'Normal' and 'Pneumonia', which contained the corresponding images. 

<br>
<br>

**Model Training** in Rekogntion is quite simple and can be done by clicking the train model button. 
<br>

![image](https://media.github.umn.edu/user/22682/files/4e6360a3-151b-4e56-8f20-a80e1307dfe0)


**Model Evaluation** can be done as below Rekogntion provides F1, Precision and Recall scores to the check the efficacy of your classification results. 

<br>

![image](https://media.github.umn.edu/user/22682/files/2f6ecff7-b5c1-4504-a83b-aa7e248b3d38)

<br>
For the deployment of your model, Rekogntion provides as an output: Python Scripts and AWS CLI Commands. We will choose the specific model we want to deploy and find the API code to start the model. Then, we can paste the API code into command line interface, here we just use AWS CloudShell, which is a browser-based command line interface within AWS system. By using AWS Cloudshell, there is no need to install any other components. 
<br>

<br>

We have created a demo for this tool, available at the following YouTube link: https://youtu.be/fRjV2iSkuLc

**Contact Us:**
<br>
Chien-Chu Hsu: hsu00122@umn.edu
<br>
Pankhuri Tyagi: tyagi040@umn.edu
<br>
Samarth Patil: patil154@umn.edu
<br>
Sarasija Gaddameedi: gadda015@umn.edu
<br>
Varun Gupta: gupta330@umn.edu
<br>
Yutian Sun: sun00503@umn.edu
<br>
