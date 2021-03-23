# Thesis - Advanced Deep Learning for Whale detection in VHR Satellite Images
Github repo for my Masters Thesis. The full details of the thesis is in the file "Thesis_Paper/Rabbani_Rabbir.pdf".

## Thesis Goals
This thesis was started with trying to answer the following questions -
1. Can Deep Learning be used to identify whales in the Very High Resolution images of satellites?
2. Can the same model be used to identify whales in comparatively lower resolution images? If it is achievable, then up to what resolution can whales be detected?
3. Can the models be used to highlight areas of interest that contain whales in an image?

## Solution Approach
1. Create a sliding window of (32*32) pixels.
2. For all the windows in an image.
  - If the Neural Network determines that the window has a whale then mark that window as 1, or else 0.
3. Draw a red border around all windows that are marked as 1.

## Implementation
Chapter 4 in the thesis paper explains how the detection was Implemented. While the Solution approach seems fairly simple, the real challenge was organizing and preprocessing the datasets, and also training several models in order to determine the best model fit for the job.

### Organizing datasets



