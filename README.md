# Fabric Defects Detector

## Introduction
The most common problem with manual inspection would be human errors while detecting the defects and calculating the correct lengths to cut. This will lead to higher wastage of fabric when cutting. This is a simple solution to detect defects in plain colored fabrics using OpenCV library. This uses contours to identify the defects on plain colored fabrics and calculates the total wastage of fabric due to the defects.

## Approach
1. Get the video stream of the fabric moving through the machine.
2. Break the video into frames.
3. Convert the frames to grayscale.
4. Apply gaussian blur to reduce the noise.
5. Convert the resulting image to binary image.
6. Apply morphology close operation to close the gaps between pixels.
7. Calculate contours.
8. Calculate the bounding rectangle for each contour.
9. Calculate the wastage by using the calculated values and the minimum piece length.
10. Show the results.

## Screenshots
![Identified defects](/screenshots/1.jpg)

![Wastage](/screenshots/2.jpg)