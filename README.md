# DICOM-3D-Vizualization
This program visualizes medical images in DICOM format, which are often used in medical scanners such as CT and MRI.
Loading DICOM Files: The pydicom library is used to read files with the .dcm extension, which contain medical images. The program assumes that these files are located in the current directory of Google Colab.

Extracting Pixel Data: The program loads pixel data from each DICOM file and stores it in the list all_images. Then all images are converted into a three-dimensional numpy array called pixels_volume, which represents the volume image.

Creating and Configuring Animation:

The program uses the plotly library to create an interactive 3D visualization.
Each image in pixels_volume is represented as a separate "frame" (go.Frame) for animation.
The initial state of the animation displays the first surface (initial_surface) of the volume data.
Interactive Controls:

The program creates an interactive slider using ipywidgets, allowing the user to select different slices of the volume image.
The function update_slider updates the displayed image when the slider position changes.
Building and Launching the Animation:

The program sets up animation control buttons, such as "Play," for automatic playback.


![](https://github.com/Artempug/DICOM-3D-Vizualization/blob/main/Untitled7.ipynb%20-%20Colab%20-%20Google%20Chrome%202024-07-27%2011-46-49%20(online-video-cutter.com).gif)

