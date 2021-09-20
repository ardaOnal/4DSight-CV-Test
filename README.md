# 4DSight-CV-Test
4DSight Computer Vision test

I tried to solve by using solvePnP and use the 2D-3D correspondences however, I could not conclude the solution therefore, I took another approach where I did not use the 2D-3D correspondences. I got the idea for the solution from a matlab function [relativeCameraPose](https://www.mathworks.com/help/vision/ref/relativecamerapose.html#d123e153998). It basically calculates the Essential matrix by finding matching points in two images and calculates the relative pose from the essential matrix. You can view the code in the file [test.py](https://github.com/ardaOnal/4DSight-CV-Test/blob/main/test.py).

Here are the results I obtained:

Solution for camera pose of img1 w.r.t. img2
Rotation matrix:
[[ 9.99999950e-01 -3.09285770e-04 -6.75795189e-05]
 [ 3.09306087e-04  9.99999907e-01  3.00834443e-04]
 [ 6.74864688e-05 -3.00855331e-04  9.99999952e-01]]
Translation vector:
[[-0.99437761]
 [-0.00196422]
 [-0.105874  ]]


Solution for camera pose of img1 w.r.t. img3
Rotation matrix:
[[ 0.99993147 -0.01081621  0.00447939]
 [ 0.01084994  0.99991243 -0.00757684]
 [-0.00439704  0.00762493  0.99996126]]
Translation vector:
[[-0.99264354]
 [ 0.02753369]
 [-0.11790126]]
 


Epipolar lines and matched points of img1-img2 & img1-img3:
![res1-2 1](https://user-images.githubusercontent.com/63498645/134078659-71e2534b-45cd-402a-b41e-78cc3a819ac8.png)
![res1-2 2](https://user-images.githubusercontent.com/63498645/134078670-121b0559-cc17-418d-a36c-9a95e5ce3131.png)
![res1-3 1](https://user-images.githubusercontent.com/63498645/134078695-46b66873-a058-42f2-8559-071734254822.png)
![res1-3 2](https://user-images.githubusercontent.com/63498645/134078632-84a4cea0-eede-4e06-83e7-d5adf94d2a43.png)






