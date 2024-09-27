## Green Screen Replacement using Python, MediaPipe, and OpenCV
Project Overview
This project demonstrates how to replace the background of a green screen video using Python, OpenCV, MediaPipe, and several other essential libraries. The pipeline uses machine learning models to segment the foreground from the background and replace the background with an image or video of your choice.

## Table of Contents
Requirements<br>
Installation<br>
How It Works<br>
References<br>

## Requirements
Python 3.x<br>
OpenCV (opencv-python)<br>
MediaPipe<br>
Numpy<br>
tqdm<br>
stow<br>
TensorFlow 2.x (tensorflow==2.*)<br>
tf2onnx<br>
onnxruntime<br>

## Installation

Clone the repository:

git clone https://github.com/SRIRAM-53-hash/Green-Screen-Replacer.git
cd green-screen-replacement

python3 -m venv env
source env/bin/activate 

## Install the required packages:

pip install -r requirements.txt
requirements.txt should contain:

makefile
Copy code
opencv-python
mediapipe
numpy
tqdm
stow
tensorflow==2.*
tf2onnx
onnxruntime

## How It Works
The project performs the following steps:

Green Screen Removal: Using OpenCV, the green screen background is identified and isolated based on a color range.

Foreground Segmentation: MediaPipe or TensorFlow models can be used to segment the human (or other subject) from the green screen, providing a cleaner background replacement.

Background Replacement: Once the foreground subject is isolated, the background is replaced by either an image or blur image or white background.

Optimization: ONNX Runtime is used to accelerate TensorFlow models by converting them into ONNX format and performing inference faster.

## References
OpenCV Documentation<br>
MediaPipe Documentation<br>
TensorFlow 2.x Documentation<br>
