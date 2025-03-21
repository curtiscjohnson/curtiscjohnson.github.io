---
title: "Real-Time Image Replacement via Homography"
layout: single-portfolio
excerpt: "SIFT Feature extraction and detection for real-time image replacement. <br/><br/><img src='/images/matches_bounding_homography.png' width='500'>"
collection: projects
---

This code for this project is available [here](https://github.com/curtiscjohnson/robotic_vision/tree/main/homography) on Github.

For this project I used the SIFT feature extraction and detection algorithm to find features in a reference image and a target image. I then used the RANSAC algorithm to find the homography matrix that best aligns the reference image with the target image. The homography matrix is then used to warp the reference image to the target image. This is useful for augmented reality applications where you want to replace a target image with a reference image in real-time.

![features](/images/matches_bounding_homography.png "features")


Here's the final result where I replace the image of the research poster with the Mona Lisa:


<iframe width="560" height="315" src="https://www.youtube.com/embed/0PKlAGML8Oc?si=Nk71DuQ38pnS4UFw" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>





