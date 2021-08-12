---
layout: post
title: Spotting difference in images
---

In this minimalistic demo ([github.com/konvica/spot-img-diff](https://github.com/konvica/spot-img-diff)), I demonstrated a simple method to localize differences between misaligned images. For example highlighting differences between screenshots of a webpage, which can be useful for Web UI Testing.
<p align="center">
    <img src="/images/spot_diff.png" height="400px"/>
</p>

This simple method is based on Computer Vision techniques. First step is image alignment, which is especially important for webpage screenshots due to scrolling up or down. I am using OpenCV Feature Matching to get coordinates of matching keypoints/regions between two images. From these coordinates I calculate homography transformation to align both images. Afterwards a simple difference between images spots different pixels. Found differences can be clustered together simply by using closing operation. In case of regions with text data, PyTesseract can be used to extract differences in text. 

<p align="center">
    <img src="/images/spot_diff2.png" height="400px"/>
</p>

