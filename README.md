# Frame quality assessment
# Assessing frame quality for a vehicle damage detection algorithm: Project overview 
* Creating a tool to assess video frame quality for a specific machine learning algorithm.
* Running fast deep learning models on videos to extract a confidence metric for each selected vehicle part using non-max suppression.
* Applying this tool to reduce data flow at the input of the semantic segmentation algorithm. 
* Deploying the model.

## Running state of the art object detection models at 110 FPS :
We are applying yolov5s on a per-frame basis in real-time! Our goal is to explore ways to stabilize the video results before reducing frames based on the confidence levels.


<p align="center">
<img src="https://github.com/aymanemoataz/Monk-AI---Data-quality-assessment/blob/master/readme_images/gif2.gif" width="450px" height="430px">


</p>

## Model 3 : yolov5s 

### Dataset

### Results

<p align="center">
<img src="https://github.com/aymanemoataz/MonkxMines_Demo/blob/master/Results_Model3/results.png" width="550px" height="330px">
</p>

#### Confusion Matrix ( We narrowed down the initial classes (60+ vehicle parts to 9 classes)
We saw that that the model confused bumper_back and bumper_front in videos with moving cars, given that position detectors can locate the back of the car we will combine the two classes in the next model.
we also work with stable cars. We are constructing a database of videos where we move around the car(suitable to the app).

<p align="center">
<img src="https://github.com/aymanemoataz/MonkxMines_Demo/blob/master/Results_Model3/confusion_matrix.png" width="550px" height="330px">


</p>




