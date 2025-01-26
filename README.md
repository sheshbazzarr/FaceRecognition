# Face Recognition Project

## Overview
This project implements a face recognition system using machine learning techniques. The primary goal is to detect and crop faces from images, which can then be used for further analysis or training of recognition models.

## Project Structure
The project is organized into several directories and files:

- `1_data_process.ipynb`: Jupyter Notebook for processing images, detecting faces, and saving cropped images.
- `data/`: Directory containing input images categorized into `male` and `female` subdirectories.
- `crop_data/`: Directory where cropped face images are saved after processing.
- `model/`: Directory containing the Haar Cascade classifier model for face detection.
- `notebooks/`: Directory containing other notebooks for different stages of the project, including:
  - `2_Train_FaceRecognition_with_ML.ipynb`: Jupyter Notebook for training a face recognition model using machine learning techniques.
  - `3_Evaluate_FaceRecognition_Model.ipynb`: Jupyter Notebook for evaluating the performance of the trained face recognition model.
  - `4_Deploy_FaceRecognition_Model.ipynb`: Jupyter Notebook for deploying the trained face recognition model in a real-world application.


## Requirements
To run this project, you will need the following Python packages:

- `numpy`
- `opencv-python`
- `matplotlib`
You can install the required packages using pip:

## Usage
1. **Prepare Your Data**: Place your images in the `data/female/` and `data/male/` directories.
2. **Run the Notebook**: Open `1_data_process.ipynb` in Jupyter Notebook and execute the cells sequentially. The notebook will:
   - Load images from the specified directories.
   - Detect faces using the Haar Cascade classifier.
   - Crop and save the detected faces into the `crop_data/females/` and `crop_data/males/` directories.

3. **Check Output**: After processing, the cropped images will be saved in the respective directories. You can verify the number of images processed by checking the output in the notebook.




## Notes
- Ensure that the Haar Cascade model file is correctly placed in the `model/` directory.
- The project is designed to handle images in `.jpg` format. Ensure your input images are in this format.
- The code includes error handling for unreadable images, which will be logged in the output.

## License
This project is licensed under the MIT License. See the LICENSE file for more details.

## Acknowledgments
- OpenCV for computer vision tasks.
- Jupyter Notebook for interactive coding and visualization.
- `IMDB-WIKI Dataset`: A large dataset of celebrity images, which can be used for training and testing face recognition models. You can download the dataset from [here](https://data.vision.ee.ethz.ch/cvl/rrothe/imdb-wiki/).
