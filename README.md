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
### Developed By: J . RITHANIEPRIYANKA
### Register Number: 212220230039
i) #To Read,display the image
```
import cv2
color_image=cv2.imread('rithu.jpg',1)
cv2.imshow('colorimage',color_image)
cv2.waitKey(0)
cv2.destroyAllWindows()

```
ii) #To write the image
```
cv2.imwrite('mountain.jpg',color_image)
cv2.imshow('mountain',color_image)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
iii) #Find the shape of the Image
```
import cv2
color_image=cv2.imread('rithu.jpg',-1)
print(color_image.shape)
```
iv) #To access rows and columns

```
import cv2
import random
color_img=cv2.imread('rithu.jpg',1)
for i in range(180):
    for j in range(color_img.shape[1]):
        color_img[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
        cv2.imshow('212220230039, J . Rithaniepriyanka',color_img)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
v) #To cut and paste portion of image
```
cut=color_image[260:280,100:300]
color_image[60:80,100:300]=cut
cv2.imshow('cutimage',color_image)
cv2.waitKey(0)
cv2.destroyAllWindows()
```

## Output:

### i) Read and display the image


![DI - EXP 1 A](https://user-images.githubusercontent.com/75235132/161386715-853d6418-433e-4c37-9e35-0cf89ae0ea89.png)

### ii)Write the image

![DI - EXP 1 B](https://user-images.githubusercontent.com/75235132/161386731-c69d65d5-5efe-4799-9b8b-bcedc0ba9128.png)

### iii)Shape of the Image

![DI - EXP 1 CODE](https://user-images.githubusercontent.com/75235132/161386739-d096154d-5e11-4907-9f41-e60de07bf1de.png)


### iv)Access rows and columns

![DI - EXP 1 C](https://user-images.githubusercontent.com/75235132/161386744-9590e5f8-26eb-48a8-8952-566aa03aaaaf.png)

### v)Cut and paste portion of image
![DI - EXP 1 D](https://user-images.githubusercontent.com/75235132/161386755-ff25f86f-5bc1-40de-8afb-2e5219112d12.png)


## Result:
Thus the images are read, displayed, and written successfully using the python program.


