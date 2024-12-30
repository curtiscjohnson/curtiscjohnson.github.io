---
title: "Robo Grader"
layout: single-portfolio
excerpt: "This project uses SIFT feature matching and some computer vision techniques to automatically grade scantrons. <br/><br/><img src='/images/feature_matching_blue.png' width='500'>"
collection: projects
---

The purpose of this project is to eliminate the need for fancy scantron grading machines. Instead, we can use computer vision techniques to grade a scantron with bubbles filled in. 

The code for this project is [here.](https://github.com/curtiscjohnson/robotic_vision/tree/main/image_registration)

The first step is to use the SIFT feature matching algorithm to find the features in the reference scantron and match them to the student's scantron. 

![features](/images/feature_matching_blue.png "features")

Since there are a lot of possible features, I used the RANSAC algorithm to find the homography matrix that best aligns the reference scantron with the student's scantron. This is called image registration.

Once the scantrons are registered, I can use the homography matrix to warp the reference scantron to the student's scantron. This allows me to compare the bubbles filled in by the student to the correct answers. Some quick image processing isolates the bubbles filled in by the student.

![features](/images/answer_field_grid_red.png "features")

Finally, I can compare the student's answers to the correct answers. I did this by dividing up each area of interest into the individual bubbles and then comparing the pixel values of the student's scantron to the reference scantron. The red numbers indicate each grid's sum of pixel values.

![features](/images/grid_sums_blue.png "features")



