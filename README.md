# camera_calibration
I forked a camera_calibration repository that gives a well structured implementation of opencv findcheckerboard. 

# Camera Intrinsic properties
[This analytics vidya link](https://www.analyticsvidhya.com/blog/2021/10/a-comprehensive-guide-for-camera-calibration-in-computer-vision/)https://www.analyticsvidhya.com/blog/2021/10/a-comprehensive-guide-for-camera-calibration-in-computer-vision/ Gives a good summary of camera intrinsics and distortion with good pics.

THese Telegram articles [Part1](https://www.tangramvision.com/blog/camera-modeling-exploring-distortion-and-distortion-models-part-i)https://www.tangramvision.com/blog/camera-modeling-exploring-distortion-and-distortion-models-part-i [Part2](https://www.tangramvision.com/blog/camera-modeling-exploring-distortion-and-distortion-models-part-ii)https://www.tangramvision.com/blog/camera-modeling-exploring-distortion-and-distortion-models-part-ii [Part3](https://www.tangramvision.com/blog/camera-modeling-exploring-distortion-and-distortion-models-part-iii)https://www.tangramvision.com/blog/camera-modeling-exploring-distortion-and-distortion-models-part-iii Explains distortions and sites the papers that mention the distortions and the algorithms


Cyrill Stachniss mentions DLT method for Camera Intrinsics and extrinsics combined. 
Need to know its functioning. I think its formulating projection matrix and solving it linearly by using Pseudo inverse method.

[Purdue notes Lecture 21](https://engineering.purdue.edu/kak/computervision/ECE661Folder/Lecture21.pdf)https://engineering.purdue.edu/kak/computervision/ECE661Folder/Lecture21.pdf explains Zhang's Algorithm which is default implementation in opencv goes by the function name findCheckercorners. anuragvvworkspace has some example implementations of the algorithm. You should know how to quickly write this algorithm.
anuragvvworkspace has GUI implementation 


[Deep Learning for Camera Calibration and Beyond: Survey](https://arxiv.org/pdf/2303.10559.pdf) mentions some previous survey papers and sumeries and tabulates deep learning methods for calibration.
***Need to implement some deep learning camera calibration and understand its working.

