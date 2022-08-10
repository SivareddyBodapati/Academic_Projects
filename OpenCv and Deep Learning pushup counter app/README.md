# OpenCv and Deep Learning Fitness Tracker app
# Idealistic Goal:
The project main goal is to build and deploy a fitness tracker app that can aslo be used remote as a zoom filter.
# Proof of Concept:
**Background Work**:
1. Generating the Data
2. Building a Deep Learning Classifier
3. Pass the Classifier to MediaPipe
4. Tracks the count, duration and calories
**Output**:
1. Deploy the App 
2. Check the Result
# Data Generation
1. Image extracted from online Youtube videos are used as the dataset
2. 500 Images of each PushUp and Situp are extracted
**frametaker.py** used for the Image Extraction
![image](https://user-images.githubusercontent.com/86652676/184018461-3312770d-4e69-43ee-ae67-481209137366.png)
![image](https://user-images.githubusercontent.com/86652676/184018815-37f8177e-3988-4ea7-a985-7e11d0d93cc4.png)

3. The extracted images are converted to skeleton images using OpenCV MediaPipe
**PoseModule_final.py** used to convert to skeleton images
