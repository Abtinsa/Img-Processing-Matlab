# 🌊 Flash Flood Detection in Iran Using Image Processing
## 📌 Overview
### This MATLAB project applies advanced image processing techniques to detect flash flood swamps in Iran. 🌍 Inspired by NASA's [Flash Floods Swamp Iran](https://earthobservatory.nasa.gov/images/149325/flash-floods-swamp-iran) article Flash Floods Swamp Iran, we analyze satellite images to highlight affected regions.
#
# 🛠️ Methodology
## 📷 1. Initial Visualization
### ✅ Display the first satellite image (December 2021).
### ✅ Load and compare it with the second image (January 2022) using a side-by-side montage.

## 🎨 2. Image Preprocessing

### ✅ Convert the second flood image to grayscale.
### ✅ Display the grayscale histogram for intensity distribution.
### ✅ Adjust contrast for better feature visibility & compare before vs. after.

![photo-collage png](https://github.com/user-attachments/assets/be7fc30a-510e-41e0-b6bf-6504118dee10)



## 🎯 3. Flood Area Detection

### ✅ Apply color thresholding on the 2021 image to segment flooded regions.
### ✅ Calculate affected area:
* Use `regionprops()` to get the area in **pixels**.
* Convert pixels to square kilometers using map scale:
```matlab
px2km = (70/100)^2; % Convert pixels to km² based on satellite resolution
areaKmSq = round(AreaPixels * px2km);
```
![photo-collage png-2](https://github.com/user-attachments/assets/f0e7a930-689f-491a-b54f-0bfda8edba1e)

## 📊 4. Data Visualization

### ✅ Bar chart 📊 to compare flood-affected areas over the years.
### ✅ Montage 🎨 to display all segmented flood areas side-by-side.
#
# 🎡 Results & Impact

### 📌 This project successfully detects and quantifies flood-affected areas. 
### 🌍 The method can be extended to future flood analysis using satellite imagery & MATLAB.
## ✨ Author  

👨‍💻 **Abtin Aghasadeghi**  
📍 Civil Engineer | Image Processing Enthusiast  
📧 [Contact Me](mailto:aghasadeghiabtin@gmail.com)  
