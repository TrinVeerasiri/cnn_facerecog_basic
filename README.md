# Face recognition using Convolution Neural Network

Test the performance of Neural network. Working from end to end. Start from collecting the data. We capture the face of 3 person with different background using Logitecth webcam C525. We separate into 450 images in training set and 50 in test set. Design the Covolution Neural Network (CNN) receives the 32x32 input images. The first layer is convolution layer with 32 3x3 filters. Feed the process images through 2x2 max pooling and pass them to second convolution layer with 32 3x3 filters. Then flatten it to fully connected layer. We use 'adam' as optimizer and 'categorical_crossentropy' as loss (because the output is more than 2). The result is 1x3 one hot encoder matrix such as [0, 1, 0]. The index of maximum value tell us the name of the person.

Thre are 3 notebooks here. <br>
1) Image Capture <br>
Run the live video feed then press 's' to save the image to specify folder. <br>
https://github.com/TrinVeerasiri/cnn_facerecog_basic/blob/master/cap_pic.ipynb
2) Train CNN <br>
https://github.com/TrinVeerasiri/cnn_facerecog_basic/blob/master/train_faces.ipynb <br>
3) Test the CNN in real-time action <br>
https://github.com/TrinVeerasiri/cnn_facerecog_basic/blob/master/face_recog.ipynb

The saved model file is <br>
https://github.com/TrinVeerasiri/cnn_facerecog_basic/blob/master/face_recog_3faces.h5

# Conclusion
Testing with live camera, result is good when moving our face closer to the camera because it's similar to the picture in train set. The performance on live may improve by increasing the training sample. Capturing face with different background and various angle. Selecting a test set is important too. Similarity between test set and image capture from live feed will help us know a real performance when using this application.  
