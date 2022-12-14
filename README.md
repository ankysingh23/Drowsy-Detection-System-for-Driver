# Drowsy-Detection-System-for-Driver π΄ π« π
In this Python project, we will be using OpenCV for gathering the images from webcam and feed them into a Deep Learning model which will classify whether the personβs eyes are βOpenβ or βClosedβ. The approach we will be using for this Python project is as follows :

Step 1 β Take image as input from a camera.

Step 2 β Detect the face in the image and create a Region of Interest (ROI).

Step 3 β Detect the eyes from ROI and feed it to the classifier.

Step 4 β Classifier will categorize whether eyes are open or closed.

Step 5 β Calculate score to check whether the person is drowsy.

Project Prerequisites π¨βπ¬
You need to have Python installed on your system, then using pip, you can install the necessary packages.

    OpenCV β pip install opencv-python (face and eye detection).
    TensorFlow β pip install tensorflow (keras uses TensorFlow as backend).
    Keras β pip install keras (to build our classification model).
    Pygame β pip install pygame (to play alarm sound).

β­ Letβs understand how our algorithm works β­

π Take Image as Input from a Camera

    With a webcam, we will take images as input.

π Detect Face in the Image and Create a Region of Interest (ROI)

    To detect the face in the image 
    we need to first convert the image into grayscale as the OpenCV 
    algorithm for object detection takes gray images in the input.
    We donβt need color information to detect the objects. 
    We will be using haar cascade classifier to detect faces. T

π Detect the eyes from ROI and feed it to the classifier

    The same procedure to detect faces is used to detect eyes..

π Classifier will Categorize whether Eyes are Open or Closed

π  Calculate Score to Check whether Person is Drowsy

    The score is basically a value we will use to determine how 
    long the person has closed his eyes. 
    So if both eyes are closed, we will keep on increasing score 
    and when eyes are open, we decrease the score.
