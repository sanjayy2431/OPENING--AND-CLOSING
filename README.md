# OPENING--AND-CLOSING
## NAME : SANJAY V
## REG NO : 212223230188
## DATE : 3/11/25
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
NAME : SANJAY V
REG NO : 212223230188
```

```

import cv2
import numpy as np
import matplotlib.pyplot as plt
image = np.zeros((500, 500, 3), dtype=np.uint8)
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(image, 'Open and Close', (100, 250), font, 1, (255, 255, 255), 2, cv2.LINE_AA)
kernel = np.ones((3, 3), np.uint8)
plt.subplot(1, 3, 1)
plt.imshow(cv2.cvtColor(image, cv2.COLOR_BGR2RGB))
plt.title("Input Image")
plt.axis('off')
plt.subplot(1, 3, 2)
plt.imshow(cv2.cvtColor(opened_image, cv2.COLOR_BGR2RGB))
plt.title("Opening Operation")
plt.axis('off')
plt.subplot(1, 3, 3)
plt.imshow(cv2.cvtColor(closed_image, cv2.COLOR_BGR2RGB))
plt.title("Closing Operation")
plt.axis('off')



```
## Output:

### Display the input Image

![image](https://github.com/user-attachments/assets/9df2b859-659f-4840-b019-d7ec5e4baa21)


### Display the result of Opening

![image](https://github.com/user-attachments/assets/45540813-1cdb-4712-81e6-204970d387eb)


### Display the result of Closing

![image](https://github.com/user-attachments/assets/757576a6-6f08-4a2d-992a-2253215aa602)


## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
