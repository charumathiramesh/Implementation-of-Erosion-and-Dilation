# Implementation-of-Erosion-and-Dilation
## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary packages.


### Step2:
Create the Text using cv2.putText.

### Step3:
Create the structuring element.

### Step4:
Erode and Dilate the image.

### Step5:
End Program.

 
## Program:

``` Python
NAME : CHARUMATHI R
REF NO : 212222240021
# Import the necessary packages
import cv2
import numpy as np
import matplotlib.pyplot as plt



# Create the Text using cv2.putText

img1=np.zeros((100,500),dtype='uint8')
font=cv2.FONT_HERSHEY_COMPLEX

# Create the structuring element
cv2.putText(img1,'CHARUMATHI' ,(5,70),font,3.3,(255),5,cv2.LINE_AA)
plt.imshow(img1,cmap='gray')
kernel1=cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))

# Erode the image
img_erode=cv2.erode(img1,kernel1)
plt.imshow(img_erode,cmap='gray')



# Dilate the image
img_dilate=cv2.dilate(img1,kernel1)
plt.imshow(img_dilate,cmap='gray')




```
## Output:

### Display the input Image
![download](https://github.com/charumathiramesh/Implementation-of-Erosion-and-Dilation/assets/120204455/33499d00-a375-4aa4-a4f1-0c1171e9e08b)


### Display the Eroded Image
![download](https://github.com/charumathiramesh/Implementation-of-Erosion-and-Dilation/assets/120204455/4698293e-0849-49e7-9cea-53845512c267)

### Display the Dilated Image

![download](https://github.com/charumathiramesh/Implementation-of-Erosion-and-Dilation/assets/120204455/82ecb8d4-c048-46d3-b97f-6386384a0fc4)

## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
