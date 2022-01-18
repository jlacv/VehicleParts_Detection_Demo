# Frame quality assessment
# Assessing frame quality for a vehicle damage detection algorithm: Project overview 
* Creating a tool to assess video frame quality for a specific machine learning algorithm.
* Running fast deep learning models on videos to extract a confidence metric for each selected vehicle part using non-max suppression.
* Applying this tool to reduce data flow at the input of the semantic segmentation algorithm. 
* Deploying the model.

## Running state of the art object detection models at 110 FPS :
We are applying yolov5s on a per-frame basis in real-time! Our goal is to explore ways to stabilize the video results before reducing frames based on the confidence levels.


<p align="center">
<img src="https://github.com/aymanemoataz/Monk-AI---Data-quality-assessment/blob/master/readme_images/gif2.gif" width="550px" height="530px">

<img src="https://github.com/aymanemoataz/Monk-AI---Data-quality-assessment/blob/master/readme_images/carside_day1.gif" width="550px" height="530px">

</p>


## Code and Resources Used 

**Pytorch**

**Python Version:** 3.9 

**For requirements:**  ```pip install -r requirements.txt```   





