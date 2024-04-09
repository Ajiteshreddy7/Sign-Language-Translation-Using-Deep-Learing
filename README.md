# Sign-Language-Translation-Using-Deep-Learing

In this project, we use CNN to convert ASL(American Sign Language) into text in real-time. The dataset was completely built from scratch.

# Dataset link: https://drive.google.com/drive/folders/1cS1Avu6k7AMiL7OqQQ9itCeU6eSSd8ET?usp=sharing

# Steps to implement the project -->
1. Install TensorFlow and Mediapipe as these two are more than sufficient because they have all the packages we need to seamlessly execute the code.
2. Run the collectdata.py and when the camera opens place your hand in the ROI(Region of Interest), then press the alphabet on the keyboard to start capturing the photos.
   Ex: make the sign "A" and press and hold on the alphabet "A" on your keyboard to continuously capture the images and save them in a folder "A".
3. Later on, Run the functions.py code, this code has all the necessary functions that are required and can be called back when needed.
4. Run the data.py code to preprocess your data i.e. convert your raw data to usable/ trainable data for the model. This code resizes the images, converts them into greyscale, and then with the help of a pre-trained model from the media pipe detects the landmarks and key points on the hands and saves those key points as JPEG images.
5. Now, use this preprocessed data to train the model. run the model.py code and set the path to the preprocessed dataset. After the model has been trained successfully and you are satisfied with your accuracy percentage.
6. Run the main.py in cmd to execute the project.
