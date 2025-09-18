---
title: Ohm-Snap
seo_title: A program for visually assessing the resistance (in ohms) of a resistor.
summary: "Our project for CruzHacks: using computer vision and machine learning to estimate the resistance of a resistor from just a phone picture."
description: "Ohm-Snap is a hackathon project built at CruzHacks. It leverages computer vision and machine learning to classify and estimate resistor resistance values directly from images, making electronics testing more accessible and convenient."
slug: ohm-snap
author: bearcbass

date: 2024-01-21T15:55:33-08:00
lastmod: 
expiryDate: 
publishDate: 

feature_image: threethreebands.jpeg
feature_image_alt: "Image alt description"

project types:
  - Machine Learning
  - Computer Vision

techstack:
  - Python
  - PyTorch
  - OpenCV

live_url: 
source_url: https://github.com/bearcbass/Ohm_Snap

newsletter: false
---

# Ohm-Snap!

This was our project for CruzHacks 2024. We wanted to create a program that could take a picture of a resistor and through that calculate the resistance in Ohms. 

My work was focused on the computer vision portion, attempting to use OpenCV to process these images and retain the spatial dimensions of the bands on the resistors while effectively preserving their color in the proper order. 

In the end we used Meta's SAM (Segment Anything Model) to handle the segmentation, which was able to properly segment the bands. However with lack of time we were not able to complete the rest of the project.

Here's a showcase of our progress. We started with an image of resistors found online, then processed it through SAM to segment the resistor body.

<div style="text-align: center; margin: 20px 0;">
  <img src="threethreebands.jpeg" alt="Original Image" style="max-width: 95%; height: auto; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">
</div>

After segmentation, we obtained the resistor with the color bands preserved. We then performed bit multiplication on the original image to maintain the resistor with its original colors. 
<div style="text-align: center; margin: 20px 0;">
  <img src="result_image.jpg" alt="Result Image" style="max-width: 95%; height: auto; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">
</div>

Finally, we used SAM again to differentiate and isolate the individual color bands on the resistors. 

<div style="text-align: center; margin: 20px 0;">
  <img src="asdf.png.jpeg" alt="Additional Image" style="max-width: 95%; height: auto; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">
</div>

