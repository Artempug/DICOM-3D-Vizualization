# DICOM-3D-Visualization

This repository provides a program for visualizing medical images in DICOM format, commonly used in medical imaging devices like CT and MRI scanners.

---

## **Features**

### **1. Loading DICOM Files**
- Utilizes the **pydicom** library to read `.dcm` files containing medical images.  
- Assumes the DICOM files are stored in the **current working directory** (e.g., Google Colab).

### **2. Extracting Pixel Data**
- Loads pixel data from each DICOM file into a list called `all_images`.  
- Converts the list into a **3D numpy array** (`pixels_volume`) representing the volumetric image.

### **3. 3D Visualization**
- Employs the **plotly** library for interactive 3D rendering.  
- Each slice in the `pixels_volume` is visualized as a "frame" (`go.Frame`) within an animation.  
- The initial state displays the first surface (`initial_surface`) of the 3D volume.

### **4. Interactive Controls**
- Adds an **interactive slider** using `ipywidgets`, enabling the user to navigate through slices of the volume.  
- A function, `update_slider`, dynamically updates the displayed image based on the slider's position.

### **5. Animation Setup**
- Includes playback controls, such as **"Play"**, to automate the visualization for an enhanced viewing experience.

---

## **Getting Started**

### **Dependencies**
- `pydicom`
- `numpy`
- `plotly`
- `ipywidgets`

### **Usage**
1. Place `.dcm` files in the specified directory.
2. Run the script in **Google Colab** or your local environment.
3. Explore and interact with the 3D visualization via the slider or animation controls.

---

This program simplifies the process of analyzing complex medical images, providing an intuitive way to explore DICOM data interactively.


![](https://github.com/Artempug/DICOM-3D-Vizualization/blob/main/Untitled7.ipynb%20-%20Colab%20-%20Google%20Chrome%202024-07-27%2011-46-49%20(online-video-cutter.com).gif)

