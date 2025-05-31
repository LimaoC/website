---
title: "Super Resolution for Satellite Imagery"
summary: "Enhancing satellite imagery resolution with state-of-the-art machine learning vision models"
date: "2024-06-02"
tags: ["machine learning"]
readTime: true
---

| | | |
|:-------------------------:|:-------------------------:|:-------------------------:|
| ![Low res](/projects/super-resolution-for-satellite-imagery/low-res.png "Low resolution")                | ![Ground truth high res](/projects/super-resolution-for-satellite-imagery/high-res.png "Ground truth high resolution") | ![Bicubic interpolation](/projects/super-resolution-for-satellite-imagery/bicubic.png "Bicubic interpolation") |
| ![MSE Autoencoder](/projects/super-resolution-for-satellite-imagery/ae-mse.png "Autoencoder (MSE loss)") | ![Perceptual Autoencoder](/projects/super-resolution-for-satellite-imagery/ae-vgg.png "Autoencoder (perceptual loss)") | ![SR-GAN](/projects/super-resolution-for-satellite-imagery/srgan.png "SR-GAN")                                 |

Super-resolution is the generative machine learning task of enhancing image resolution while retaining important visual structures and features. Many state-of-the-art computer vision models, such as Generative Adversarial Networks (Ledig et al., 2017), autoencoders (Dong et al., 2015), and diffusion models (Ho, Jain, and Abbeel, 2020), have been successfully applied to super-resolution tasks. These tasks have applications in many domains, such as medical imaging, computer vision, and satellite imagery (Froede, 2023). In this report, we explore these state-of-the-art (SOTA) models on satellite imagery from the Sentinel-2 and VENμS satellites.

High-resolution satellite imagery can be used for monitoring land cover changes, deforestation, and disaster response, among many other applications (Njambi, 2023). As such, it would be desirable to have a satellite that combines the strengths of both Sentinel-2 and VENμS and captures high-resolution imagery at a global scale. However, deploying a new satellite with these attributes would be costly. Instead, we apply SOTA models to bridge this gap and simulate globally available high-resolution satellite imagery.

The SEN2VENμS dataset is an open-data licensed dataset of landscape images (patches) from the Sentinel-2 and VENμS satellites which have been physically aligned and have undergone pre-processing stages. Sentinel-2 has a global range but limited resolution, whereas VENμS has a limited range, but is capable of capturing images at a higher resolution. More specifically, the Sentinel-2 images have a resolution of 128×128 pixels, whereas the VENμS images have a resolution of 256×256 pixels, so our super resolution task has an upscaling factor of two. While there are papers in the literature (Lanaras et al., 2017; Lin and Bioucas-Dias, 2020; Paris, Bioucas-Dias, and Bruzzone, 2017) that have applied super-resolution to imagery from these satellites individually, we will need to use imagery from both satellites to upscale the Sentinel-2 imagery to the resolution capability of VENμS as performed between Sentinel-2 and Rapid-Eye (Galar et al., 2019), which is a fairly novel task for our satellites (Michel et al., 2022).

This is a STAT3007 group project that I worked on in 2024 Semester 1.

---

* <a href="/projects/super-resolution-for-satellite-imagery/report.pdf" target="_blank">Full Report</a>
* <a href="https://github.com/LimaoC/super-resolution-for-satellite-imagery" target="_blank">GitHub</a>
* <a href="https://www.mdpi.com/2306-5729/7/7/96" target="_blank">Original dataset paper</a>
* <a href="https://zenodo.org/records/6514159#.YoRxM5PMK3I" target="_blank">Original dataset</a>
