Crack Detection Project
This project is aimed at building a visual analysis pipeline for detecting and inspecting cracks in images. The code allows for image distribution analysis, sample visualization, mask overlay, size verification, pixel intensity plotting, and edge detection, providing valuable insights into the characteristics of crack images.

Table of Contents
Project Description
Setup Instructions
Functionality Overview
Class Distribution
Sample Image Display
Image and Mask Display
Image Size Verification
Pixel Intensity Plot
Edge Detection Visualization
Dependencies
Usage
Project Description
This project analyzes and processes images in two classes: Positive (images with cracks) and Negative (images without cracks). It includes utilities for image visualization, distribution plotting, and edge detection to aid in crack identification tasks.

Here's a sample README content for your crack detection project repository on GitHub. This README covers the description, setup instructions, and functions available in your script:

Crack Detection Project
This project is aimed at building a visual analysis pipeline for detecting and inspecting cracks in images. The code allows for image distribution analysis, sample visualization, mask overlay, size verification, pixel intensity plotting, and edge detection, providing valuable insights into the characteristics of crack images.

Table of Contents
Project Description
Setup Instructions
Functionality Overview
Class Distribution
Sample Image Display
Image and Mask Display
Image Size Verification
Pixel Intensity Plot
Edge Detection Visualization
Dependencies
Usage
Project Description
This project analyzes and processes images in two classes: Positive (images with cracks) and Negative (images without cracks). It includes utilities for image visualization, distribution plotting, and edge detection to aid in crack identification tasks.

Setup Instructions
Clone the repository:
bash
Copy code
git clone https://github.com/your-username/crack-detection.git
Navigate to the repository directory:
bash
Copy code
cd crack-detection
Install the required packages:
bash
Copy code
pip install -r requirements.txt
Functionality Overview
1. Class Distribution
Displays the distribution of positive and negative images in the dataset.

python
Copy code
# Run this to view class distribution
plt.bar(['Positive', 'Negative'], [num_positive, num_negative])
2. Sample Image Display
Displays a sample of images from each class for visual inspection.

python
Copy code
display_sample_images(image_dirs=[positive_dir, negative_dir], labels=['Positive', 'Negative'], num_samples=5)
3. Image and Mask Display
Visualizes images, their masks, and overlays the mask on the original image to highlight crack areas.

python
Copy code
display_images_with_masks(image_dir=positive_dir, mask_dir=mask_dir, num_samples=5)
4. Image Size Verification
Displays histograms of the width and height of images to ensure consistency across the dataset.

python
Copy code
verify_image_sizes(image_dirs=[positive_dir, negative_dir])
5. Pixel Intensity Plot
Plots the distribution of pixel intensities across a subset of images, which can help in understanding the grayscale intensity range of cracks.

python
Copy code
plot_pixel_intensity(image_dirs=[positive_dir, negative_dir], num_samples=100)
6. Edge Detection Visualization
Applies edge detection to sample images for identifying crack boundaries.

python
Copy code
edge_detection_visualization(image_dir=positive_dir, num_samples=5)
Dependencies
Ensure you have the following packages installed:

numpy
opencv-python
matplotlib
pandas
Usage
To run the code, simply execute the script in a Python environment with access to the dataset. Make sure to specify the correct paths for the Positive and Negative directories in the script.
