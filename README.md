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
### Developed By:PRAKASH R
### Register Number: 212222240074
i) #To Read,display the image
```
  import cv2
img = cv2.imread('flower.png', 0)
resized_img = cv2.resize(img, None, fx=0.8, fy=0.8)
cv2.imshow('212222240025', resized_img)
cv2.waitKey(0)
cv2.destroyAllWindows()

  

```
ii) #To write the image
```

import cv2
img=cv2.imread('flower.png',0)
cv2.imwrite('writed_walt.png',img)




```
iii) #Find the shape of the Image
```

import cv2
img=cv2.imread('flower.png',0)
print(img.shape)




```
iv) #To access rows and columns

```import cv2
img = cv2.imread('flower.png', 0)
resized_img = cv2.resize(img, None, fx=0.8, fy=0.8)
for i in range(100, 250):
    for j in range(10, 50):
        resized_img[i][j] = 255  
cv2.imshow('212222240025', resized_img)
cv2.waitKey(0)
cv2.destroyAllWindows()



```
v) #To cut and paste portion of image
```

import cv2
img = cv2.imread('flower.png', 1)
tag = img[300:400, 300:400]
img[50:150, 50:150] = tag
cv2.imshow('212222240025', img)
cv2.waitKey(0)





```

## Output:

### i) Read and display the image

<br> 

<br>


### iv)Access rows and columns
<br>

<br>![dip ex 1 op img 1](https://github.com/prakash22004108/READ-AND-WRITE-IMAGE/assets/113497032/2693d680-42b2-492d-86c3-d578c6d4d4dd)


### v)Cut and paste portion of image
<br>
![image](https://github.com/prakash22004108/READ-AND-WRITE-IMAGE/assets/113497032/4c8d4201-ad78-4372-b1c4-a506f06dd18f)

<br>

## Result:
Thus the images are read, displayed, and written successfully using the python program.
