# Driver-Drowsiness-Detection
Drowsiness detection is a safety technology that can prevent accidents that are caused by drivers who fell asleep while driving.

Here We've used OpenCV, Tensorflow, Keras and Pygame to build a programme that triggers alarm if the driver is drowsy and prevents a calamity from happening in a live video feed. We've used a CNN model using keras involving the following layers, to train a dataset to classify between closed and open eyes. (Model.py)<br>
The model is then saved to models/cnnCat2.h5.<br>
Then the programme to detect a drowsy driver uses OpenCV Haarcascade function to detect the eyes of the driver, our ROI, and then applies our CNN model to the ROI, and predicts a score, saying the driver is drowsy or not. If the core is above certain mark, the programm triggers an audio alarm using pygame. (drowsiness detection.py)<br>
Here is a sample Drowsy Driver Detected Image.
