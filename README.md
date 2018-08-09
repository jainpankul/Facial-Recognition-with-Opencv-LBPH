## Facial-Recognition-with-OpenCV-LBPH

When we talk about face recognition, we basically need to do two things:

Face Detection - finding a face in an image
Face Recognition - determining who the person is
There are many techniques for face recognition like Eigen Faces, Fisher Faces, Local Binary Patterns Histograms (LBPH), neural network.

For our purpose, we are going to use Haar Classifier for face detection and LBPH for face recognition.

For more details on how Haar Classifier and LBPH works, please see https://docs.opencv.org/2.4/modules/objdetect/doc/cascade_classification.html https://docs.opencv.org/2.4/modules/contrib/doc/facerec/facerec_tutorial.html#local-binary-patterns-histograms

We are going to divide the entire process in 4 parts:

* Data Preparation - Storing the images of each person in separate folder and label them
* Face Detection - Running Haar Classifier on each image and detect face.
* Training LBPH Face recognizer - Training the recognizer on stored data
* Prediction - check if the face recognizer predicts correctly on test images

For data preparation, I have stored the images of Tom Cruise and Hilliary Clinton in different folders and label them 1 and 2 respectively.
