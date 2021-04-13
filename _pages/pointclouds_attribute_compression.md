---
title: "Point clouds - attribute compression"
author_profile: true
layout: single
sidebar:
  nav: "projs"
classes: wide
permalink: /point-clouds-attribute-compression/
---

Point cloud data is generally represented by a list of voxels, each being described by its geometry (location in space) and attributes (RGB or YUV color spaces, luminance etc.). The Group has developed several attribute compression technologies:

## Region-Adaptive Hierarchical Transform

<p style="text-align:center;">
  <img src="https://github.com/DiogoCaetanoGarcia/minimal-mistakes/raw/master/assets/images/RAHT.png"><br>
  <i>Illustration of RAHT in a 2x2x2 block</i><br>
</p>

The Region-Adaptive Hierarchical Transform (RAHT) is a hierarchical sub-band transform that resembles an adaptive variation of a Haar wavelet. It is currently adopted by MPEG’s [Geometry-based Point Cloud Compression (G-PCC) standard](https://ieeexplore.ieee.org/document/8571288).

### Publications

* R. L. de Queiroz and P. A. Chou, "[Compression of 3D point clouds using a region-adaptive hierarchical transform](http://queiroz.divp.org/papers/ieee_tip_raht3d.pdf)," IEEE Trans. on Image Processing, Vol. 25, No. 8, pp. 3497-3956, Aug. 2016.
* G. A. Sandri, P. A. Chou, M. Krivokuca, R. L. de Queiroz, "[Integer alternative for the region-adaptive hierarchical transform](http://queiroz.divp.org/papers/ieee_spl_integer_raht.pdf)," IEEE Signal Processing Letters, Vol. 26, No. 9, pp. 1369-1372, Sep. 2019.
* G. Sandri, R. L. de Queiroz, and P. A. Chou, "[Comments on 'Compression of 3D Point Clouds Using a Region-Adaptive Hierarchical Transform'](https://arxiv.org/pdf/1805.09146.pdf)", arXiv:1805.09146 [eess.IV], May 2018.

### Ph.D. Thesis

* G. L. Sandri,  [Compression of Point Cloud Attributes](http://queiroz.divp.org/papers/tese_GustavoSandri_dsc.pdf), Tese de Doutorado, Universidade de Brasília, 2019.

### Software

* [Source code (MATLAB on Linux/Windows)](https://github.com/digitalivp/RAHT)

### Patent

* P. A. Chou and R. de Queiroz, "Region adaptive hierarchical transform and entropy coding for point cloud compression and corresponding decompression," March 5, 2019, U.S. Patent # 10,223,810.

## Compression of plenoptic attributes

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

* R. L. de Queiroz, C. Dorea, D. C. Garcia, R. U. Ferreira, D. R. Freitas, R.Higa, I. Seidel and V. Testoni, "Differential plenoptic point cloud codingfor  V-PCC,"  in ISO/IEC  JTC1/SC29  Joint  WG11/WG7  (MPEG/JPEG) input document WG7M55145, Online, October 2020.

### Ph.D. Thesis

* G. L. Sandri,  [Compression of Point Cloud Attributes](http://queiroz.divp.org/papers/tese_GustavoSandri_dsc.pdf), Tese de Doutorado, Universidade de Brasília, 2019.

## Other contributions

Interesting alternatives to the RAHT are the Gaussian Process Transforms (GPTs):

### Publications

* R. L. de Queiroz and P. A. Chou, "[Transform coding for point clouds using a Gaussian process model](http://queiroz.divp.org/papers/ieee_tip2017_klt.pdf)," IEEE Trans. on Image Processing, Vol. 26, No. 7, pp. 3507-3517, July 2017.
