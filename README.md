# Monk-AI---Data-quality-assessment
# Assessing Image quality for a vehicle damage detection algorithm: Project Overview 
* Creating a tool to assess image data quality for a specefic machine learning algorithm.
* Implementing a faster algorithm using machine learning techniques to eliminate non pertinent data before passing it to the vehicle damage detection model.
* Reducing Data flow and helping to optimize a machine learning model. 
* Integrating the model into a phone application. 

## Problem presentation
<img src = 'https://github.com/aymanemoataz/Monk-AI---Data-quality-assessment/blob/master/Yolo_Vehicle_Parts_Detection/00e3f8e41c.parts.jpeg' width="324" height="324">
This is an example of the company's model run on an image of low quality. We can see that the model segments the pixels in the image to recognize car parts in order to help assign the image to a particular damage class. We can see that assessing image quality is crucial to optimize the model. Integrating a Machine learning model to assess image quality in different parts of the image is essential. You can check the report and the presentation folders for details. Our approach and data will be brefiely presented below.

## Code and Resources Used 
**Python Version:** 3.9 
**ForRequirements:**  ```pip install -r requirements.txt```   
**Scraper Article:** https://towardsdatascience.com/selenium-tutorial-scraping-glassdoor-com-in-10-minutes-3d0915c6d905  


## Approach

## Data ( Webscraping | company provided data)

### Webscraping data : initial model

Tweaked a web scraper to collect 500 car images, scraping a 100 images for each keyword. I then removed some images manually and used 100 images for training and 10 images to test the yolo model at first.

* We narrowed our task to only identify 5 classes.
* The number of objects in each class is evenly distributed, knowing that we are working with car images.
* We chose objects that are distinguishable in different types of cars.

### Company provided data : optimizing the initial model

## Data preprocessing
we need to supervise yolo's learning with bounding box annotations. We draw a box around each object that we want the detector to see and label each box with the object class that we would like the detector to predict.
* We used CVAT for computer annotation in order to prepare our initial training data(webscraped data), data can be downloaded from this link : https://app.roboflow.com/ds/2minm3ukA8?key=UAcbAfF26m

<img src = 'https://github.com/aymanemoataz/Monk-AI---Data-quality-assessment/blob/master/readme_images/datapreprocessing.png' width="524" height="324">

## Initial Results :

## Validating the initial results :
We will test our quality score on zoomed car images, and car videos with angle changes to see how the quality score changes. This could help us reduce some frames from videos and understand which part is visible in a given image
