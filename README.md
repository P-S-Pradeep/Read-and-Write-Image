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
# Developed By: PRADEEP PS
# Register Number : 212220230034
# To Read,display the image
img = cv2.imread('flower.jpg',1)
cv2.imshow('nature',img)
cv2.waitKey(0)





# To write the image
grey = cv2.imread('flower.jpg',0)
cv2.imshow('nature',gray)
cv2.waitKey(0)

# To write the image

cv2.imwrite('ou2.jpg',grey)





# Find the shape of the Image
print(img.shape)




# To access rows and columns
import random
for i in range(200):
    for j in range(img.shape[1]):
        img[i][j] = [random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('flower',img)
cv2.waitKey(0)





# To cut and paste portion of image
img1 = cv2.imread('flower.jpg',1)
tag = img1[300:400:,300:400]
img1[50:150,50:150] = tag
cv2.imshow('flower',img1)
cv2.waitKey(0)










```
## Output:

### i) Read and display the image

![j2](https://user-images.githubusercontent.com/102652887/160788626-024e3163-f95f-4bb9-94f7-b22dd9781bb9.jpeg)


### ii)Write the image

![j3](https://user-images.githubusercontent.com/102652887/160788766-4d58f775-3427-4b6e-b1fc-9527790da27e.jpeg)


### iii)Shape of the Image
![j4](https://user-images.githubusercontent.com/102652887/160788838-646bb0ba-8c7a-49f2-b83a-b95e203519b8.png)


### iv)Access rows and columns
![j5](https://user-images.githubusercontent.com/102652887/160789006-4a42d85e-5509-4ed4-9c3d-189f4804877b.jpeg)


### v)Cut and paste portion of image
![j6](https://user-images.githubusercontent.com/102652887/160789179-d2fa0e69-d116-4316-94fd-0c2a564653cd.jpeg)


## Result:
Thus the images are read, displayed, and written successfully using the python program.


