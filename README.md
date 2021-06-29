# OptiTrip: Detecting Falls Using Optical Flow 
## Johns Hopkins University - Computer Vision Fall 2020 - Final Project 

Combining the complimentary signals of human-pose tracking and optical flow tracking a method is used to concentrate optical flow tracking to just the area of interest in the frame - for fall detection this is the person falling. The limitations for this method include: only one person can be falling the frame at a time (although several can be detected), the camera must be stationary, and the thresholding parameters may need minor adjustment per dataset.  

## Executable Files
**OFbased.ipynb:** Implementation of optical flow only fall detection method <br />
**humanPose.ipynb:** Implementation of human pose only fall detection method <br />
- currently set up to be executed locally (to change to Google Colab execution, see instructions before last cell) <br />

**combined_HP_OF:** implementation of combined method (human pose and optical flow)
- currently setup to be executed on colab (please upload all files in this directory into the colab directory)

## Not Executable - for reference only
**OF_cv2.ipynb:** calculated Optical Flow method statistics across both URFD and our Custom Fall dataset

## Datasets
URFD: http://fenix.univ.rzeszow.pl/~mkepski/ds/uf.html <br />
Custom Fall Dataset: https://drive.google.com/drive/folders/1MmrSGVAX_Lxq1SyO1UuayjkleycAl5nu?usp=sharing
