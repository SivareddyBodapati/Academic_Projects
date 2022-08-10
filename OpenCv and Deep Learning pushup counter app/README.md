# OpenCv and Deep Learning Fitness Tracker app
## Idealistic Goal:
The project main goal is to build and deploy a fitness tracker app that can aslo be used remote as a zoom filter.
## Proof of Concept:
### Background Work :
1. Generating the Data.
2. Building a Deep Learning Classifier.
3. Pass the Classifier to MediaPipe.
4. Tracks the count, duration and calories.
### Output:
1. Deploy the App.
2. Check the Result.
## Data Generation
1. Image extracted from online Youtube videos are used as the dataset.
2. 500 Images of each PushUp and Situp are extracted.
**frametaker.py** used for the Image Extraction.
![image](https://user-images.githubusercontent.com/86652676/184018461-3312770d-4e69-43ee-ae67-481209137366.png)
![image](https://user-images.githubusercontent.com/86652676/184018815-37f8177e-3988-4ea7-a985-7e11d0d93cc4.png)

3. The extracted images are converted to skeleton images using OpenCV MediaPipe.
**PoseModule_final.py** used to convert to skeleton images.

![image](https://user-images.githubusercontent.com/86652676/184019730-bc856162-aba5-4bb4-bc11-674106a1f638.png)
![image](https://user-images.githubusercontent.com/86652676/184019761-10c8d505-9ef5-42b9-908e-ce41767f9867.png)

## Building a Deep Learning Classifier
1. Cnn classifier from PyTorch library is trained with the preprocessed data. **Pose__classification2.ipynb** is used to define, train and evaluating the model.
2. Best model **Best_Pose_Model_7.pth** is saved and used for postprocessing and later on passed to MediaPipe. **Pose_classifier.py** is used for predictions and classifing the input image.
