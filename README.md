
# IOT Remote Control with Hand Gestures Using OpenCV & Machine-Learning (NARUTO-STYLE)

This project trains a neural network to detect hand gestures with Object-Detection and OpenCV. A series of detected hand gestures is used as logics in python to play and pause music, reduce and increase volume of music, and skip tracks on a Sonos home speaker device.

Conventionally, one would be expected to wave or make a fist at the webcam to, for example, gesture the device to start playing music. While this makes more sense, I think it lacks a tiny bit of BAAAAAA TAAAASSSSSS.

Therefore, the twist in my project, targeted at all you anime weebs, requires gesturing a series of Naruto ninja handsigns to command the device. Why? Because #ThatsMyNinjaWay #Dattebayo

## Inspiration

This hand gesture remote control using OpenCV and MachineLearning aspect of this project is inspired by various Google Mediapipe pose detection projects on the web. While the project did not use Mediapipe (because Naruto handsigns confuses Mediapipe), similar intended result is achieved with the help of transfer learning.

The Naruto handsign element, on another hand, is inspired by my previous project: [Naruto OpenCV Machine-Learning Game](https://github.com/Aspiring-DataGod9000/Naruto-OpenCV-Machine-learning-Game.git).

## Demo



https://user-images.githubusercontent.com/102948566/177460034-1cd361af-371e-4ea5-918b-2e1ed328828d.mp4




## Training the Model

1. Labelling images of myself doing the various naruto handsigns using LabelImg.

2. labelled images are seperated into train and test folders, used to train my selected machine learning model.

3. Model of choice is transfer learning model, SSD Mobilenet, as the model is versatile and yield better results than vgg16 for my project.

4. After the training of my model completed, the model was embedded into OpenCV for real time detection of handsigns

5. Finally, logics are written within OpenCV to assign different commands to each series of gestures. Interface of the gesture guide is coded in Pygame.
## Model
Model Of Choice: SSD Mobile Net

![mobileNet-SSD-network-architecture](https://user-images.githubusercontent.com/102948566/177460122-143ca192-9fb9-49d7-86fc-8f2c05e7f105.png)


Model Accuracy:

| Hand Signs | Train    | Test |
| ---------- | -------- | ---- |
| Monkey     | 85%      | 80%  |
| Dragon     | 89%      | 79%  |
| Rat        | 92%      | 87%  |
| Bird       | 98%      | 85%  |
| Snake      | 89%      | 76%  |
| Ox         | 93%      | 71%  |
| Dog        | 95%      | 80%  |
| Horse      | 99%      | 75%  |
| Tiger      | 91%      | 74%  |
| Boar       | 87%      | 70%  | 
| Ram        | 93%      | 87%  | 
| Hare       | 96%      | 90%  |

## Acknowledgements (References & Source of Inspirations)

  - [Learning with Rev - Transfer Learning Mobilenet V2 - Large Fish Project](https://www.youtube.com/watch?v=DElZ6sn3ADI)
  - [Custom Object Detection using TensorFlow from Scratch](https://towardsdatascience.com/custom-object-detection-using-tensorflow-from-scratch-e61da2e10087)
  - [Python pygame – The Full Tutorial](https://coderslegacy.com/python/python-pygame-tutorial/)
