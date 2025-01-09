---
title: "Depth-Guided Privacy-Preserving Visual Localization Using 3D Sphere Clouds"
collection: publications
category: conferences
permalink: /publication/Spherecloud
excerpt: '<img src="../images/spherecloud_generation.png" width="400" height="200"> <img src="../images/spherecloud_attack.png" width="400" height="200">'
date: 2024-11-25
venue: 'British Machine Vision Conference 2024 (BMVC 2024)'
paperurl: 'https://bmva-archive.org.uk/bmvc/2024/papers/Paper_267/paper.pdf'
# citation: 'H. Moon et al. (2024). &quot;Depth-Guided Privacy-Preserving Visual Localization Using 3D Sphere Clouds 3.&quot; <i>In proceedings of British Machine Vision Conference (BMVC 2024) </i>. 1(3).'
---

# Sphere-cloud
## [BMVC 2024] Depth-Guided Privacy-Preserving Visual Localization Using 3D Sphere Cloud
**Authors:** **Heejoon Moon**, Jongwoo Lee, Jeonggon Kim, [Je Hyeong Hong](https://sites.google.com/view/hyvision)

**[[Paper](https://bmva-archive.org.uk/bmvc/2024/papers/Paper_267/paper.pdf)][[Project Page](https://bmvc2024.org/proceedings/267/)]** 
<!-- [[Code](https://github.com/PHANTOM0122/Sphere-cloud)] -->

<video width="640" height="480" controls>
  <source src="../images/spherecloud1.mp4" type="video/mp4">
  동영상을 재생할 수 없습니다.
</video>
<video width="640" height="480" controls>
  <source src="../images/spherecloud2.mp4" type="video/mp4">
  동영상을 재생할 수 없습니다.
</video>

The emergence of deep neural networks capable of revealing high-fidelity scene details from sparse 3D point clouds has raised significant privacy concerns in visual localization involving private maps.
Lifting map points to randomly oriented 3D lines is a well-known approach for obstructing undesired recovery of the scene images, but these lines are vulnerable to a density-based attack that can recover the point cloud geometry by observing the neighborhood statistics of lines.
With the aim of nullifying this attack, we present a new privacy-preserving scene representation called \emph{sphere cloud}, which is constructed by lifting all points to 3D lines crossing the centroid of the map, resembling points on the unit sphere.
Since lines are most dense at the map centroid, the sphere cloud mislead the density-based attack algorithm to incorrectly yield points at the centroid, effectively neutralizing the attack. 
Nevertheless, this advantage comes at the cost of i) a new type of attack that may directly recover images from this cloud representation and ii) unresolved translation scale for camera pose estimation.
To address these issues, we introduce a simple yet effective cloud construction strategy to thwart new attack and 
 propose an efficient localization framework to guide the translation scale by utilizing absolute depth maps acquired from on-device time-of-flight (ToF) sensors.
Experimental results on public RGB-D datasets demonstrate sphere cloud achieves competitive privacy-preserving ability and localization runtime while not excessively compensating the pose estimation accuracy compared to other depth-guided localization methods.

