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
### Developed By: Gayathri A
### Register Number: 212221230028
i) #To Read,display the image
```
import cv2
import matplotlib.pyplot as plt
img=cv2.imread('gayu.jpg',1)
cv2.imshow('moon',img)
cv2.waitKey(0)
```
ii) #To write the image
```
import cv2
A=cv2.imread("gayu.jpg",1)
cv2.imwrite("gayu.jpg",A)
cv2.imshow("moon",A)
cv2.waitKey(0)


```
iii) #Find the shape of the Image
```
import cv2
moon=cv2.imread('gayu.jpg',1)
print(moon.shape)

```
iv) #To access rows and columns

```
import random
import cv2
A=cv2.imread("gayu.jpg",1)
for i in range(100):
    for j in range(A.shape[1]):
        A[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow("moon",A)
cv2.waitKey(0)



```
v) #To cut and paste portion of image
```
import cv2
A=cv2.imread("gayu.jpg",1)
tag=A[140:240,165:180]
A[25:125,50:65]=tag
cv2.imshow("moon",A)
cv2.waitKey(0)

```

## Output:

### i) Read and display the image

<br>![WhatsApp Image 2023-03-16 at 12 33 27 AM](https://user-images.githubusercontent.com/94154854/225633325-35ebc129-5ace-443a-bd0f-7e82a4d663f7.jpeg)

<br>

### ii)Write the image

<br>![WhatsApp Image 2023-03-16 at 12 33 27 AM](https://user-images.githubusercontent.com/94154854/225633325-35ebc129-5ace-443a-bd0f-7e82a4d663f7.jpeg)

<br>

### iii)Shape of the Image

![WhatsApp Image 2023-03-16 at 12 33 27 AM (1)](https://user-images.githubusercontent.com/94154854/225636246-e61fd614-a814-40ba-8062-ac2516aad280.jpeg)


### iv)Access rows and columns

<br>![WhatsApp Image 2023-03-16 at 12 33 28 AM](https://user-images.githubusercontent.com/94154854/225633438-ea35b0c7-3919-46d6-8468-fd39be9a6caa.jpeg)

<br>

### v)Cut and paste portion of image

<br>![WhatsApp Image 2023-03-16 at 12 33 28 AM (1)](https://user-images.githubusercontent.com/94154854/225633545-d26c0b54-6cdf-4d56-954d-478cc47ce24a.jpeg)

<br>

## Result:
Thus the images are read, displayed, and written successfully using the python program.


