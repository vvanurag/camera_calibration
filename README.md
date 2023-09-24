# camera_calibration
I forked a camera_calibration repository that gives a well structured implementation of opencv findcheckerboard. 

# Camera Intrinsic properties
[This analytics vidya link](https://www.analyticsvidhya.com/blog/2021/10/a-comprehensive-guide-for-camera-calibration-in-computer-vision/)https://www.analyticsvidhya.com/blog/2021/10/a-comprehensive-guide-for-camera-calibration-in-computer-vision/ Gives a good summary of camera intrinsics and distortion with good pics.

THese Telegram articles [Part1](https://www.tangramvision.com/blog/camera-modeling-exploring-distortion-and-distortion-models-part-i)https://www.tangramvision.com/blog/camera-modeling-exploring-distortion-and-distortion-models-part-i [Part2](https://www.tangramvision.com/blog/camera-modeling-exploring-distortion-and-distortion-models-part-ii)https://www.tangramvision.com/blog/camera-modeling-exploring-distortion-and-distortion-models-part-ii [Part3](https://www.tangramvision.com/blog/camera-modeling-exploring-distortion-and-distortion-models-part-iii)https://www.tangramvision.com/blog/camera-modeling-exploring-distortion-and-distortion-models-part-iii Explains distortions and sites the papers that mention the distortions and the algorithms

Try to understand the mathematical modeling of the the lens effcts including focal length, dstortions(radial, tangential, ect), ect.


[Cyrill Stachniss mentions DLT method](https://www.youtube.com/watch?v=3NcQbZu6xt8) for Camera Intrinsics and extrinsics combined. 
Need to know its functioning. I think its formulating projection matrix and solving it linearly by using Pseudo inverse method.
Check out [Cyrill Stachniss Zhang method](https://www.youtube.com/watch?v=-9He7Nu3u8s) also


Cyrill says to solve the x = PX equation, If intrinsics are known, we need 6 unknowns i.e 3 points to solve. If intrinsics are unknown, then its 11 unknowns in P and needs 5.5 \~= 6 points
Cyrill in DLT method shows how we can solve for p with SVD and also how p can be decomposed into K|R using QR decomposition.
This method gives degenerate results if the 3D points are planar!!! 
Observe how Zhang's algo for planar points is different from DLT!!!
Also, Lens distortion models can also be included in the solving. Check last part of video for this info. IMPORTANT!!! 

GUI for visualizing checkerboard transform by changing intrinsic and extrinsic parameters!! ([repository](https://github.com/anuragvvworkspace/VirtualCam_camera_calibration))

[Purdue notes Lecture 21](https://engineering.purdue.edu/kak/computervision/ECE661Folder/Lecture21.pdf)https://engineering.purdue.edu/kak/computervision/ECE661Folder/Lecture21.pdf explains 
![image](https://github.com/vvanurag/camera_calibration_project/assets/22678131/6ca1de12-1d39-47f0-8fec-2a08efaf7815)

Zhang's Algorithm which is default implementation in opencv goes by the function name findCheckercorners. anuragvvworkspace has some example implementations of the algorithm. You should know how to quickly write this algorithm.
anuragvvworkspace has GUI implementation 


[Deep Learning for Camera Calibration and Beyond: Survey](https://arxiv.org/pdf/2303.10559.pdf) mentions some previous survey papers and sumeries and tabulates deep learning methods for calibration.
***Need to implement some deep learning camera calibration and understand its working.

Also have to explore multi-camera calibration and multi-sensor calibration (like LiDAR-camera calibration)



