### Project Description

> `Virtual Paint` is a simple `python` application made using `opencv` module. We can paint on the realtime screen using our fingers. 

+ We can draw on the Screen(out image) using fingers(moving in the webcam viewport area). For drawing we use our index finger open. There are 5 different colors available in this project and an eraser to erase drawn work. 

+ For selection we use our index and  middle fingers open.We can even change the brush and rubber size through the changing values in the respected variables.

> What all I used in this project :-
> + Python : `opencv`, `numpy`, time, math
> + `HandTrackingModel.py` : `openv`, `numpy`, time, math, `mediapipe`


+ The `HandTrackingModel.py` is a python file which is used to detect the fingers. You can download the `HandTrackingModel.py` from the Github repository. The link to the Github repository is [HandTrackingModel.py](https://github.com/mnk17arts/myPython/tree/main/opencv/hand-tracking-module)

+ The complex part of the project was to draw on the screen. I used the `HandTrackingModel.py` to detect the fingers and then I used the `cv2.line()` function to draw on the screen. I used the `cv2.circle()` function to draw the brush and rubber. I used the `cv2.rectangle()` function to draw the color palette.

+ The full code of this project is available at the Github repository. You can download the code from there. The link to the Github repository is [Virtual Paint](https://github.com/mnk17arts/myPython/tree/main/opencv/virtual-paint-project)

### Project Demo

> The demo of this project is available in a Video Format. You can view the demo from there. The link to the Video is [Virtual Paint Demo](https://user-images.githubusercontent.com/71878747/118365406-4c163380-b5ba-11eb-8b4f-124e1ffb665a.mp4).