# working-on-images.
# REG NO: 212222230057
# NAME: JOEL P

# Working on Images
My submission
Instructions for submission 
1. The image should be a plant, Tree, flower or building

2. The filename should be username.jpg

3. The image should be Converted to gray scale and HSV 

4. Display the H, S and V planes



## Program:
# Convert to Gray Scale and HSV:
```
import cv2
image = cv2.imread('Screenshot 2024-03-08 092502.png')
grayscale_image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
hsv_image = cv2.cvtColor(image, cv2.COLOR_BGR2HSV)
```

## ORIGINAL OUTPUT:
![Screenshot 2024-03-08 092502](https://github.com/SHARAN-MJ/Search-Algorithm/assets/119560305/ff7b5747-dbc0-4a67-9772-aebfe96a01a5)


# Display H, S, and V Planes:

```
h, s, v = cv2.split(hsv_image)

# Display the H, S, and V planes
cv2.imshow('Hue', h)
cv2.imshow('Saturation', s)
cv2.imshow('Value', v)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
# OUTPUT:

![Screenshot 2024-03-08 092752](https://github.com/SHARAN-MJ/Search-Algorithm/assets/119560305/1f80f847-9e77-4b2a-8afd-c0bad64c17e3)
![Screenshot 2024-03-08 092818](https://github.com/SHARAN-MJ/Search-Algorithm/assets/119560305/8f8afc98-3a72-4ec0-b93a-1f1618a709d0)
![Screenshot 2024-03-08 092806](https://github.com/SHARAN-MJ/Search-Algorithm/assets/119560305/1e91fe0d-87ca-446f-9b9e-98c2e501cbb0)


# Save the Processed Image:
```
cv2.imwrite('username_gray.jpg', grayscale_image)
cv2.imwrite('username_hsv.jpg', hsv_image)

```
# OUTPUT;
![Screenshot 2024-03-08 092843](https://github.com/SHARAN-MJ/Search-Algorithm/assets/119560305/0d26e761-233b-4e86-8b7c-23ab60e55846)

