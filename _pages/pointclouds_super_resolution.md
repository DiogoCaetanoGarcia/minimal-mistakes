---
title: "Point clouds - super-resolution"
author_profile: true
layout: single
sidebar:
  nav: "projs"
classes: wide
permalink: /point-clouds-super-resolution/
---

<p style="text-align:center;">
  <img src="https://github.com/DiogoCaetanoGarcia/minimal-mistakes/raw/master/assets/images/pointcloud_superresolution.png"><br>
  <i>Super-resolution framework (SR) that outputs a superresolved frame by exploring the high-frequency content similarities between a down-sampled point-cloud and a time-adjacent frame.</i><br>
</p>

The Group proposed a mixed-resolution point-cloud representation and a super-resolution framework, from which several processing tools can be derived, such as compression, denoising and error concealment. The proposed super-resolution methods work by inferring the high-frequency content of low-resolution frames based on (a) the similarities between adjacent full-resolution frames and (b) a dictionary of low- and high-frequency pairs built from adjacent full-resolution frames.

<p style="text-align:center;">
  <img src="https://github.com/DiogoCaetanoGarcia/minimal-mistakes/raw/master/assets/images/pointcloud_superresolution_example_based.png"><br>
  <i>Full example of the super-resolution of one pixel in 2D, based on the similarities between adjacent full-resolution frames.</i><br>
  <img src="https://github.com/DiogoCaetanoGarcia/minimal-mistakes/raw/master/assets/images/pointcloud_superresolution_lut.png"><br>
  <i>Building a dictionary of children nodes based on the current voxel’s neighbors.</i><br>
</p>


### Publications
* D. C. Garcia, T. A. Fonseca, R. U. Ferreira and R. L. de Queiroz, "[Geometry coding for dynamic voxelized point clouds using octrees and multiple contexts](http://queiroz.divp.org/papers/ieee_tip_lossless_octree.pdf)," IEEE Trans. on Image Processing, Vol. 29, No. 1, pp.313-322, Jan. 2020.
* D. C. Garcia, T. A. Fonseca, R. L. de Queiroz, "[Example-based super-resolution for point cloud video](http://queiroz.divp.org/papers/icip2018_tiagoSR.pdf)," Proc. IEEE Intl. Conf. Image Processing, ICIP, Athens, Greece, Oct. 2018.