# IIP-InteractiveDJ
An interactive DJ product aimed to recreate how DJs play music

## Requirements 
* **OpenCV >= 2.4**: use your preferred package manager (brew, apt), build from source using [vcpkg](https://github.com/Microsoft/vcpkg) or download from [OpenCV official site](https://opencv.org/releases.html) (on Windows set system variable `OpenCV_DIR` = `C:\opencv\build` - where are the `include` and `x64` folders [image](https://user-images.githubusercontent.com/4096485/53249516-5130f480-36c9-11e9-8238-a6e82e48c6f2.png))

## Installation
Clone this repository. Donwoload yolo-obj_final.weights (https://drive.google.com/file/d/1ZNAcg0t_hCi4tCCKAQsElsv4odEwSqLU/view?usp=sharing) and place it in the same directory as play.py. 

Use the script with the following command:
```
python play.py
```
## Gestures

### Play/Resume 

Hold one open palm.

### Pause 

Hold two closed fists. (You won't be able to puase for 3 seconds after this.)

### Next song

Hold two open fists

### Volume up
Hold two fingers in a V shape.

### Volume down

Make an ok sign.


## Notes
Some samples from the training data used can be found in traing_data_samples. For every gesture around 50 images were used for training. While I tried to do as many different poses, the background is still the same, so you might not get that good of a result when you are trying it in a different environment (I don't too when I do it somewhere other than my working desk). This is just a prototype and I am trying to show what this product can be used for, not the capabilities of YOLO.

### How do you get the weights used for detection? Can I train my own weights for something different?

I used darknet, a framework created by the authors of YOLO which can be found here: https/github.com/AlexeyAB/darknet. For training I used Google Colab, as it increases training speed by a lot. 
