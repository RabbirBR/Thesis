# Thesis - Advanced Deep Learning for Whale detection in VHR Satellite Images
Github repo for my Masters Thesis. The full details of the thesis is in the file "Thesis_Paper/Rabbani_Rabbir.pdf".

## 1 Thesis Goals
This thesis was started with trying to answer the following questions -
1. Can Deep Learning be used to identify whales in the Very High Resolution images of satellites?
2. Can the same model be used to identify whales in comparatively lower resolution images? If it is achievable, then up to what resolution can whales be detected?
3. Can the models be used to highlight areas of interest that contain whales in an image?

## 2 Background
Chapter 2 aims to provide a background to the work done in the Thesis. Please refer to this chapter in case if any terminology is not sufficiently explained in this brief explanation. 

### 3 Solution Approach
Chapter 3 discusses existing approaches and gives an overall idea of what is done in this thesis. It starts by discussing some existing methods that are used to find whales and then discussing some existing Object Detection methods

### 3.1 Proposed Solution
1. Create a sliding window of (32*32) pixels.
2. For all the windows in an image.
  - If the Neural Network determines that the window has a whale then mark that window as 1, or else 0.
3. Draw a red border around all windows that are marked as 1.

## 4 Implementation
Chapter 4 in the thesis paper explains how the detection was Implemented. While the Solution approach seems fairly simple, the real challenge was organizing and preprocessing the datasets, and also training several models in order to determine the best model fit for the job.

### 4.1 Organizing and preprocessing datasets
1. The images were split into 32*32 images and put into 2 main folders whales and not-whales.
2. They were further separated into three folders *Training*, *Validation* and *Evaluation*.
3. The images were also downsampled 5 times and put in their own folders. The spacial resolution of these downsampled images were 0.62m, 1.24m, 2.48m, 4.96m and 9.92m. Figures 4.1-4.6 show the effect of the downsampling. 

### 4.2 Training and Testing the Models
1. Four Advanced CNN Architectures were trained and tested to see which works best. They are - MobileNetV2, XceptionV1, ResNet152V2 and DenseNet201. Section 4.2 in the Thesis Paper explains in detail how the Training was implemented and the Testing setup.
2. Section 4.3 explains the how the Object detection was implemented.

## 5 Results
Chapter 5 explains the results using several images for each of the models. Please refer to this section to see the results as it is hard to explain in just text. After testing, the results showed that the best model was determined to be ResNet152V2.

## Conclusion
The original questions asked in the thesis were all confirmed to be true.

