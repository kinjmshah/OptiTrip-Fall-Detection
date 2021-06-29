# OptiTrip: Detecting Falls Using Optical Flow 
### _Johns Hopkins University - Computer Vision Fall 2020 - Final Project_

### Human Pose Estimation
_Executeable File: humanPose.ipynb_

[Detectron2](https://github.com/facebookresearch/detectron2) library used to extract human bounding box and pose keypoints. Keypoints and bounding box corners are tracked between frames to produce frame-to-frame keypoint velocity estimation.

### Optical Flow 
_Executeable File: OpticalFlow.ipynb_

Frame-to-frame optical flow calculated using tools from OpenCV. Optical flow calculated for all pixels. Average optical flow used to classify video as fall or no fall based on thresholing with a pre-set threshold.

_For Reference Only: OpticalFlow_ReferenceOnly.ipynb_
This file calculated Optical Flow method statistics across both URFD and our Custom Fall dataset - results are saved in the notebook and for reference only - this notebook will not run as required dataset are not loaded as part of the notebook

### Combined: Human Pose and Optical Flow 
_Executeable File: combined_humanPose_opticalFlow.ipynb_

The human pose and optical flow signals are combined to provide a method which addresses the sparseness of the human pose method and the sensitivity of the optical flow method to background noise. By detecting the human pose and bounding box, we are able to focus the optical flow calculations to a target region of interest (ROI). Currently, only one person can be in the frame at a time, camera must be stationary, and thresholding parameters may need to be adjusted by dataset. 

## Datasets
URFD: http://fenix.univ.rzeszow.pl/~mkepski/ds/uf.html                 
Custom Fall Dataset: For access to this dataset send a request to tevere.erica11@gmail.com and kinjmshah@gmail.com

## Notes
1. Executeable files can have two methods, either loading all files into a single root directory where the executeable notebook is located, or having access to the final project google drive. Access to the _custom fall dataset_ is needed to run the demo files. 


