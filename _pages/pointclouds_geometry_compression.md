---
title: "Point clouds - geometry compression"
author_profile: true
layout: single
sidebar:
  nav: "projs"
classes: wide
permalink: /point-clouds-geometry-compression/
---

Point cloud data is generally represented by a list of voxels, each being described by its geometry (location in space) and attributes (RGB or YUV color spaces, luminance etc.). The Group has developed several geometry compression technologies:

## Dyadic composition

<p style="text-align:center;">
  <img src="https://github.com/DiogoCaetanoGarcia/minimal-mistakes/raw/master/assets/images/dyadic_decomp.gif"><br>
  <i>Diagram showing dyadic decomposition.</i><br>
</p>

[Several point-cloud codecs](https://ieeexplore.ieee.org/document/8571288) compress the geometry information based on the octree decomposition. In dyadic decomposition, on the other hand, the point cloud geometry is viewed as an array of bi-level images, inspired by well-known techniques for coding this type of images. This array is recursively split into two arrays of half its size, transmitting the occupancy information of each smaller array. Context adaptive arithmetic coding, using both 2D and 3D contexts, is used to achieve efficient compression.

### Publications

* E. Peixoto, "[Intra-Frame Compression of Point Cloud Geometry Using Dyadic Decomposition](https://ieeexplore.ieee.org/document/8957232)," in IEEE Signal Processing Letters, vol. 27, pp. 246-250, 2020.
* E. Peixoto, E. Medeiros and E. Ramalho, "[Silhouette 4d: An Inter-Frame Lossless Geometry Coder Of Dynamic Voxelized Point Clouds](https://ieeexplore.ieee.org/document/9190648)," Proc. IEEE Intl. Conf. Image Processing, ICIP, Online, September, 2020.
* D. R. Freitas, E. Peixoto, R. L. de Queiroz and E. Medeiros, "[Lossy Point Cloud Geometry Compression Via Dyadic Decomposition](https://ieeexplore.ieee.org/document/9190910)," Proc. IEEE Intl. Conf. Image Processing, ICIP, Online, September, 2020.
* D. R. Freitas, E. Peixoto, R. L. de Queiroz, and E. Medeiros, "[Lossy point cloud geometry compression via dyadic decomposition](http://queiroz.divp.org/papers/ICIP2020_dyadic_decomp.pdf)," Proc. IEEE Intl. Conf. Image Processing, ICIP, Online, September, 2020.
* D. R. Freitas, E. Peixoto, R. L. de Queiroz e E. Medeiros, "[Estudo de perdas para codificação de geometria de nuvens de pontos por decomposição diádica](http://queiroz.divp.org/papers/SBrT_2020_LossyGeomCoder.pdf)," Anais XXXVI Simpósio Brasileiro de Telecomunicações e Processamento de Sinais, SBrT 2020, Florianópolis, Brazil, Nov. 2020.
* R. Rosário and E. Peixoto, "[Intra-Frame Compression of Point Cloud Geometry using Boolean Decomposition](https://ieeexplore.ieee.org/document/8965783)," 2019 IEEE Visual Communications and Image Processing (VCIP), Sydney, NSW, Australia, 2019, pp. 1-4.

<!--## Compression of plenoptic attributes

<p style="text-align:center;">
  <img src="https://github.com/DiogoCaetanoGarcia/minimal-mistakes/raw/master/assets/images/thai-rotate_small.gif"><br>
  <i>Plenoptic point cloud</i><br>
</p>

In real-world objects, the reflected light may significantly change with the viewing angle, especially if specular surfaces are present. For that, we are interested in a more complete representation, the plenoptic point cloud, wherein every point has associated colors in different directions.

### Publications

* G. Sandri, R. L. de Queiroz and P. A. Chou, "[Compression of plenoptic point clouds](http://queiroz.divp.org/papers/ieee_tip2018_plenopticpc.pdf)," IEEE Trans. on Image Processing, Vol. 28, No. 3, pp. 1419-1427, Mar. 2019.
* G. Sandri, R. L. de Queiroz, P. A. Chou, "[Compression of plenoptic point clouds using the Region-Adaptive Hierarchical Transform](http://queiroz.divp.org/papers/icip2018_sandri.pdf)," Proc. IEEE Intl. Conf. Image Processing, ICIP, Athens, Greece, Oct. 2018.
* G. Sandri, P. A. Chou and R. L. de Queiroz, "[Representação Compressível para codificação de nuvens de pontos plenópticas](https://biblioteca.sbrt.org.br/articles/916)," Anais XXXVI Simpósio Brasileiro de Telecomunicações e Processamento de Sinais, Campina Grande, PB, Brasil, DOI 10.14209/sbrt.2018.127, Sep. 2018.

### Submission to MPEG standards

* R. L. de Queiroz, C. Dorea, D. C. Garcia, R. U. Ferreira, D. R. Freitas, R.Higa, I. Seidel and V. Testoni, "Differential plenoptic point cloud codingfor  V-PCC,"  inISO/IEC  JTC1/SC29  Joint  WG11/WG7  (MPEG/JPEG)input document WG7M55145, Online, October 2020.

### Ph.D. Thesis

* G. L. Sandri,  [Compression of Point Cloud Attributes](http://queiroz.divp.org/papers/tese_GustavoSandri_dsc.pdf), Tese de Doutorado, Universidade de Brasília, 2019.

## Other contributions

Interesting alternatives to the RAHT are the Gaussian Process Transforms (GPTs):

### Publications

* R. L. de Queiroz and P. A. Chou, "[Transform coding for point clouds using a Gaussian process model](http://queiroz.divp.org/papers/ieee_tip2017_klt.pdf)," IEEE Trans. on Image Processing, Vol. 26, No. 7, pp. 3507-3517, July 2017.
-->