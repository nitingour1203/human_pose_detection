# human_pose_detection

<b>Human pose estimation from video plays a critical role in various applications such as quantifying physical exercises, sign language recognition, and full-body gesture control. For example, it can form the basis for yoga, dance, and fitness applications. It can also enable the overlay of digital content and information on top of the physical world in augmented reality.

## An example of a graphical skeleton is shown below:

![image](https://user-images.githubusercontent.com/48796009/228968225-7509e39c-9d41-42f5-aed9-3387ad9eaa17.png)

# So how does it work?
<b>MediaPipe uses TensorFlow lite in the backend. Using a detector first locates the person (ROI) within the frame. Then it uses the ROI cropped frame as INPUT and predicts the landmarks/key-points within the ROI. The mediaPipe pose estimator detects a total of 33 key points.

MediaPipe pose estimation is a single 3D pose estimator. It detects x, y, and z coordinates for each landmark. Z-axis is basically information about the depth of a landmark. That means how far or close the landmarks are from the camera relative to the other landmarks.

<b>MediaPipe Pose is a ML solution for high-fidelity body pose tracking, inferring 33 3D landmarks and background segmentation mask on the whole body from RGB video frames utilizing our BlazePose research that also powers the ML Kit Pose Detection API. Current state-of-the-art approaches rely primarily on powerful desktop environments for inference, whereas our method achieves real-time performance on most modern mobile phones, desktops/laptops, in python and even on the web.

![image](https://user-images.githubusercontent.com/48796009/228968898-73de4945-1957-4656-a17a-c4180c49dbe7.png)


 MediaPipe Pose real-world 3D coordinates

https://user-images.githubusercontent.com/48796009/228969800-b6e3092a-75a0-4660-9d42-e02f6f4ff4e5.mp4



## Pose Estimation Quality

To evaluate the quality of our models against other well-performing publicly available solutions, we use three different validation datasets, representing different verticals: Yoga, Dance and HIIT. Each image contains only a single person located 2-4 meters from the camera. To be consistent with other solutions, we perform evaluation only for 17 keypoints

![image](https://user-images.githubusercontent.com/48796009/228968792-c3da1cd4-7b18-4d57-ab2c-482825deccd6.png)


## Categories of human pose detection:


1. 2D pose estimation: In 2d pose estimation only the x and y coordinates are predicted for each landmark in an image. It doesn’t give any information about the skeleton’s angles or the rotation or orientation of an object or human instance.

2. 3D pose estimation: 3d pose estimation allows us to predict the spiral position of a human. It gives x, y, and z coordinates for each landmark. With 3d pose estimation, we can determine the angle of each joint of a human skeleton.

3. Rigid pose estimation: Rigid pose estimation is also known as 6D pose estimation. It provides all information about the human pose as well as the rotation and orientation of a human instance.

4. Single pose estimation: In a single pose estimation model only one human’s pose can be predicted in an image.

5. Multi pose estimation: In multi-pose estimation, Multiple human poses can be predicted in an image at the same time.

# Human Pose detection with OpenCV Output:

![image](https://user-images.githubusercontent.com/48796009/228970042-859e9c76-01f5-434d-b65d-5be6c19eda36.png)
