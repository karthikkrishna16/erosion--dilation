# Reg.No:212223240067
# Name: TH KARTHIK KRISHNA
# Implementation-of-Erosion-and-Dilation
## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
### Algorithm:
#### Step1:<br>
Import the necessary pacakages

#### Step2:<br>
Create the text using cv2.putText

#### Step3:<br>
Create the structuring element

#### Step4:<br>
Erode the image


#### Step5: <br>
Dilate the Image

 
## Program:

# Import the necessary packages
````
import cv2
import numpy as np
import matplotlib.pyplot as plt
````

# Create the Text using cv2.putText
````
def load_img():
    blank_img=np.zeros((600,600))
    font=cv2.FONT_HERSHEY_SIMPLEX
    cv2.putText(blank_img,"ABCDE",(50,300),fontFace=font,fontScale=5,color=[255,255,255],thickness=25,lineType=cv2.LINE_AA)
    return blank_img
````


# Create the structuring element
````
image = load_img()
plt.imshow(image, cmap='gray')
plt.show()
````

# Erode the image
````
kernel=np.ones((5,5),np.uint8)
kernel
ersion=cv2.erode(image,kernel,iterations=4)
plt.imshow(ersion,cmap='gray')
````

# Dilate the image
````
dilution=cv2.dilate(image,kernel,iterations=4)
plt.imshow(dilution,cmap='gray')
````



## Output:

### Display the input Image

<img width="601" height="514" alt="Screenshot 2025-10-09 134932" src="https://github.com/user-attachments/assets/7d997597-b279-411f-904f-ec31fc154188" />


### Display the Eroded Image

<img width="584" height="551" alt="Screenshot 2025-10-09 134941" src="https://github.com/user-attachments/assets/836acb75-904c-4dce-bbee-e9b1136cea23" />

### Display the Dilated Image

<img width="617" height="527" alt="Screenshot 2025-10-09 134948" src="https://github.com/user-attachments/assets/96a4ce13-5cdd-461f-abb5-75e405c6ab5f" />


## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
