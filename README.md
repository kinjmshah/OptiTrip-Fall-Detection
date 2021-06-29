# OptiTrip: Detecting Falls Using Optical Flow 
### _Johns Hopkins University - Computer Vision Fall 2020 - Final Project_
### Human Pose Estimation
_Executeable File: humanPose.ipynb_

[Detectron2](https://github.com/facebookresearch/detectron2) library used to extract human bounding box and pose keypoints. Keypoints and bounding box corners are tracked between frames to produce frame-to-frame keypoint velocity estimation.

### Optical Flow 
_Executeable File: OpticalFlow.ipynb_

Combining the complimentary signals of human-pose tracking and optical flow tracking a method is used to concentrate optical flow tracking to just the area of interest in the frame - for fall detection this is the person falling. The limitations for this method include: only one person can be falling the frame at a time (although several can be detected), the camera must be stationary, and the thresholding parameters may need minor adjustment per dataset.  

## Executable Files
**OFbased.ipynb:** Implementation of optical flow only fall detection method <br />
**humanPose.ipynb:** Implementation of human pose only fall detection method <br />
- currently set up to be executed locally (to change to Google Colab execution, see instructions before last cell) <br />

**combined_HP_OF:** implementation of combined method (human pose and optical flow)
- currently setup to be executed on colab (please upload all files in this directory into the colab directory)

## For Reference Only
**OF_cv2.ipynb:** calculated Optical Flow method statistics across both URFD and our Custom Fall dataset - results are saved in the notebook and for reference only - this notebook will not run as required dataset are not loaded as part of the notebook

## Datasets
URFD: http://fenix.univ.rzeszow.pl/~mkepski/ds/uf.html <br />
Custom Fall Dataset: For access to this dataset send a request to tevere.erica11@gmail.com and kshah31@jhu.edu

