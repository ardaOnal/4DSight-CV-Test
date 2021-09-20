# 4DSight-CV-Test
4DSight Computer Vision test

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
 

Epipolar lines of img1-img2 and img1-img3
![img1-img2](https://user-images.githubusercontent.com/63498645/134076133-1e8d79f8-7f76-44b8-8087-4ab917d613bc.png)
![img1-img3](https://user-images.githubusercontent.com/63498645/134076146-5ef760bb-cd1e-4f83-bf4c-02984b6b202e.png)

Tried to solve using solvePnP and use the 2D-3D correspondences however, I could not conclude the solution therefore, I took another approach where I did not use the 2D-3D correspondences. I got the idea from a matlab function [relativeCameraPose](https://www.mathworks.com/help/vision/ref/relativecamerapose.html#d123e153998).
