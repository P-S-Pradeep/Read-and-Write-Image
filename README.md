# READ AND WRITE AN IMAGE
## AIM
To write a python program using OpenCV to do the following image manipulations.
i) Read, display, and write an image.
ii) Access the rows and columns in an image.
iii) Cut and paste a small portion of the image.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Choose an image and save it as a filename.jpg
### Step2:
Use imread(filename, flags) to read the file.
### Step3:
Use imshow(window_name, image) to display the image.
### Step4:
Use imwrite(filename, image) to write the image.
### Step5:
End the program and close the output image windows.
## Program:
```python
# Developed By: Tamil Venthan R S
# Register Number:212220230054
# To Read,display the image
import cv2
bw=cv2.imread("jp.jpeg",1)
cv2.imshow('212220230054-TamilVenthan RS',bw)


cv2.waitKey(0)




# To write the image

cv2.imwrite("newimage.jpeg",bw)





# Find the shape of the Image

print(bw.shape)


# To access rows and columns

import random
for i in range(100):
    for j in range(bw.shape[1]):
        bw[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('accessing row and column',bw)
cv2.waitKey(0)



# To cut and paste portion of image

bw2=cv2.imread("jp.jpeg",1)
tag=bw2[100:150,100:190]
bw2[30:80,30:120]=tag
cv2.imshow("cutting portion",bw2)
cv2.waitKey(0)

```
## Output:

### i) Read and display the image

<br>

![ex1 1](https://user-images.githubusercontent.com/75235477/160865594-ab4bccc5-99e5-4769-a8dd-6e3cc1a42d40.png)
<br>
### ii)Write the image

<br>
![ex1 2](https://user-images.githubusercontent.com/75235477/160865694-671048f4-8ac7-4983-b130-608b63916a0f.png)

<br>

### iii)Shape of the Image

<br>
![ex1 3](https://user-images.githubusercontent.com/75235477/160865728-2b192e15-657d-4a24-89e2-875b03176906.png)

<br>

### iv)Access rows and columns
<br>
<br>

### v)Cut and paste portion of image
<br>
<br>

## Result:
Thus the images are read, displayed, and written successfully using the python program.


