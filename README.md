# Frame quality assessment
# Assessing frame quality for a vehicle damage detection algorithm: Project overview 
* Creating a tool to assess video frame quality for a specefic machine learning algorithm.
* Runing fast deep learning models on videos to extract a confidence metric for each selected vehicle part using non-max suppression.
* Applying this tool to reduce data flow at the input of the semantic segmentation algorithm. 
* Deploying the model.

## Running state of the art object detection models at 76 FPS :
We are applying yolov5s on a per-frame basis in real-time! Our goal is to explore ways to stabilize the video results before reducing frames based on the confidence levels.

![Game Process](https://github.com/aymanemoataz/Monk-AI---Data-quality-assessment/blob/master/Images/git3.gif)



## Code and Resources Used 

**Pytorch**

**Python Version:** 3.9 

**For requirements:**  ```pip install -r requirements.txt```   





