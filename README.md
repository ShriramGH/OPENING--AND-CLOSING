# OPENING-AND-CLOSING
## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary packages
### Step2:
Create the Text using cv2.putText
### Step3:
Create the structuring element

### Step4:
Use Opening operation

### Step5:
Use Closing Operation

## Program:
```
Developed by: Shriram S
Register Number:212222240098
```
### Display the input Image
```py
import cv2
import numpy as np

img=np.zeros((100,400), dtype='uint8')
font=cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img,'Shriram S',(5,70), font,2,(255),5,cv2.LINE_AA)
cv2.imshow('Sample', img)
cv2.waitKey(0)
```
### Create the structured element
```py
struct_ele = np.ones((9, 9), np.uint8)
```
### Display the result of Opening
```py
opening = cv2.morphologyEx(img, cv2.MORPH_OPEN, struct_ele)
cv2.imshow('Opening', opening)
cv2.waitKey(0)
```
### Display the result of Closing
```py
closing = cv2.morphologyEx(img, cv2.MORPH_CLOSE, struct_ele)
cv2.imshow('Closing', closing)
cv2.waitKey(0)
```
## Output:

### Display the input Image

![EX_10-OP-1](https://github.com/ShriramGH/OPENING--AND-CLOSING/assets/117991122/cbb46a1e-a491-4e78-8a13-d3d9ae15ef90)


### Display the result of Opening

![Ex_10-OP-2](https://github.com/ShriramGH/OPENING--AND-CLOSING/assets/117991122/f755bf24-93ba-4fcb-b83d-b6aad624acd1)


### Display the result of Closing

![Ex_10-OP-3](https://github.com/ShriramGH/OPENING--AND-CLOSING/assets/117991122/464a56cf-21e1-4368-8d84-a25a159de187)


## Result

### Thus the Opening and Closing operation is used in the image using python and OpenCV.
