# A NOVEL CENTROID UPDATE APPROACH FOR CLUSTERING-BASED SUPERPIXEL METHODS AND SUPERPIXEL-BASED EDGE DETECTION
This project introduces an innovative approach to superpixel generation and edge detection in image processing. It builds upon the concept of [Simple Non-Iterative Clustering](https://openaccess.thecvf.com/content_cvpr_2017/papers/Achanta_Superpixels_and_Polygons_CVPR_2017_paper.pdf) (SNIC) and introduces an enhanced version with a novel centroid update mechanism. This README provides instructions for setting up and running the project, along with a brief overview of the standard and enhanced SNIC methods.

### Standard SNIC
SNIC is a method used for segmenting an image into superpixels. It starts by placing a grid of initial cluster centers across the image, with each pixel assigned to the nearest cluster based on color similarity and spatial proximity. The cluster centers are updated to be the mean of all pixels in the cluster. SNIC is known for its efficiency and simplicity.

### Enhanced SNIC
The enhanced version of SNIC introduced in this project utilizes a novel centroid update approach. It calculates two centroids for each superpixel: a coordinate centroid (mean of the coordinates of all the pixels in the superpixel) and a color centroid (mean of all the colors within an adaptively sized square around each cluster center). This approach allows for a more nuanced and accurate representation of superpixels, adapting to the local color diversity of the image.

![Screenshot from 2023-12-14 16-02-16](https://github.com/rhuthik/Improved-SNIC/assets/59531096/3bd0f17d-a4bc-4ee3-997c-5bc8b519fd7e)

## Instructions for running the file
It is adviced to create a virtual environment to run the project GUI
we can create this using the virtualenv command
```
virtualenv venv
```
(If virtualenv is not installed it can installed using 
```
sudo apt install virtualenv
```
Now we can activate this virtualenv with the following command
```
source ./venv/bin/activate
```
## Installing Dependencies
The project requires several libraries including numpy, OpenCV, matplotlib, scikit-image, Tkinter, tqdm, and Pillow. Install them using pip:
```
pip install cv2 matplotlib scikit-image tk tqdm pillow
```
## Running the Project
After installing the dependencies, you can run the project using:
```
python main.py
```

Input images link: https://drive.google.com/file/d/1_kar5hPmEayHrrKJq6btGvr5eTnDgDuh/view?usp=sharing

## Results
![Screenshot from 2023-12-14 16-01-16](https://github.com/rhuthik/Improved-SNIC/assets/59531096/8bb662ee-5bc0-481b-b13b-057275ccf4bd)

