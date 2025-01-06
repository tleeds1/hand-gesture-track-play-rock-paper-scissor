# hand-gesture-tracking-to-play-rock-paper-scissor
Estimate hand pose using MediaPipe (Python version).<br>
<br> ❗ _️**This is a version that adjust and improve from [original repo](https://github.com/Kazuhito00/hand-gesture-recognition-using-mediapipe) that train the model and make gameplay paper-rock-scissor.**_ ❗
<br> 
Special thanks to the English translation version from the original repo. <br>
The English version of the original repo is at Nikita Kiselov(https://github.com/kinivi)
![mqlrf-s6x16](https://user-images.githubusercontent.com/37477845/102222442-c452cd00-3f26-11eb-93ec-c387c98231be.gif)

This repository contains the following contents.
* Sample program
* Hand sign recognition model(TFLite)
* Finger gesture recognition model(TFLite)
* Learning data for hand sign recognition and notebook for learning
* Learning data for finger gesture recognition and notebook for learning

# Requirements
* mediapipe 0.8.1
* OpenCV 3.4.2 or Later
* Tensorflow 2.3.0 or Later<br>tf-nightly 2.5.0.dev or later (Only when creating a TFLite for an LSTM model)
* scikit-learn 0.23.2 or Later (Only if you want to display the confusion matrix) 
* matplotlib 3.3.2 or Later (Only if you want to display the confusion matrix)

# Demo
Here's how to run the demo using your webcam.
```bash
python app.py
```

The following options can be specified when running the demo.
* --device<br>Specifying the camera device number (Default：0)
* --width<br>Width at the time of camera capture (Default：960)
* --height<br>Height at the time of camera capture (Default：540)
* --use_static_image_mode<br>Whether to use static_image_mode option for MediaPipe inference (Default：Unspecified)
* --min_detection_confidence<br>
Detection confidence threshold (Default：0.5)
* --min_tracking_confidence<br>
Tracking confidence threshold (Default：0.5)

# How to use:
## Select Mode
* --k<br>Training mode for hand gesture.
* --h<br>Training mode for finger gesture.
* --p<br>Playing mode for paper rock scissors game

For more information about way to train, visit [original repo](https://github.com/Kazuhito00/hand-gesture-recognition-using-mediapipe) or [translated version](https://github.com/kinivi/hand-gesture-recognition-mediapipe)
# Reference
* [MediaPipe](https://mediapipe.dev/)

# Author of Original Repo:
Kazuhito Takahashi(https://twitter.com/KzhtTkhs)

# Translation
Nikita Kiselov(https://github.com/kinivi)

# Author of this repo
Tho Le Doan(https://github.com/tleeds1)

# License 
this project is under [Apache v2 license](LICENSE).
