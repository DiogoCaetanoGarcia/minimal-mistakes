---
title: "Face spoofing detection"
author_profile: true
layout: single
sidebar:
  nav: "projs"
classes: wide
permalink: /miscellaneous-face-spoofing-detection/
---

<p style="text-align:center;">
  <img src="https://github.com/DiogoCaetanoGarcia/minimal-mistakes/raw/master/assets/images/face_spoofing.png"><br>
  <i> Moiré patterns due to the overlapping of digital grids. (a) Portion of the Lena test image. (b) Photograph of (a) on a 13-inch Macbook Pro screen and shot by an iPhone 4 camera without any compression artifacts. (c)-(d) Details of (a)-(b), respectively. (e)-(f) Absolute values of the discrete Fourier transforms of (a)-(b).</i><br>
</p>

Biometric systems based on face recognition have been shown unreliable under the presence of face-spoofing images. Hence, automatic solutions for spoofing detection became necessary. The Group proposed face-spoofing detection by searching for Moiré patterns due to the overlap of the digital grids, and developed an image database of facial shots under several conditions.

<p style="text-align:center;">
  <img src="https://github.com/DiogoCaetanoGarcia/minimal-mistakes/raw/master/assets/images/image_recapture.png"><br>
  <i>Image recapture: a screened image is captured by an imaging system
from a distance.</i><br>
  <img src="https://github.com/DiogoCaetanoGarcia/minimal-mistakes/raw/master/assets/images/image_recapture.png"><br>
  <i>Samples of the Moiré database.</i><br>
</p>


### Publications

* D. C. Garcia and R. L. de Queiroz, "[Face-spoofing 2D-detection based on Moiré-pattern analysis](http://queiroz.divp.org/papers/ieee_tifs_face_spoofing.pdf)," IEEE Trans. on Information Forensics and Security, Vol. 10, No. 4, pp. 778-786, April 2015.
* D. C. Garcia and R. L. de Queiroz, "[Evaluating the effects of image compression in Moire-pattern-based face-spoofing detection](http://queiroz.divp.org/papers/icip2015diogo.pdf)," Proc. IEEE Intl. Conf. on Image Processing, ICIP, Quebec City, Canada, Sep. 2015.

### Database

* Repository containing a face-spoofing database with images of 50 individuals captured under 13 different conditions: [link](https://gitlab.com/diogogarcia/Moire_database)