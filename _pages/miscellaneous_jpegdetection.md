---
title: "Recolorization"
author_profile: true
layout: single
sidebar:
  nav: "projs"
classes: wide
permalink: /miscellaneous-jpeg-detection/
---

<p style="text-align:center;">
  <img src="https://github.com/DiogoCaetanoGarcia/minimal-mistakes/raw/master/assets/images/jpegdetect1.png"><br>
  <img src="https://github.com/DiogoCaetanoGarcia/minimal-mistakes/raw/master/assets/images/jpegdetect2.png"><br>
  <img src="https://github.com/DiogoCaetanoGarcia/minimal-mistakes/raw/master/assets/images/jpegdetect3.png"><br>
</p>

Sometimes image processing units inherit images in raster bitmap format only, so that processing is to be carried without knowledge of past operations that may compromise image quality (e.g., compression). To carry further processing, it is useful to not only know whether the image has been previously JPEG compressed, but to learn what quantization table was used. This is the case, for example, if one wants to remove JPEG artifacts or for JPEG re-compression. We developed fast and efficient methods to determine whether an image has been previously JPEG compressed and to estimate compression parameters via a maximum likelihood estimation of JPEG quantization steps. We further explored JPEG Compression History Estimation through a statistical dictionary-based and  blind lattice-based algorithms. Our work is frequently cited in image forensics articles dealing with JPEG compression.

### Publications


* Z. Fan and R. de Queiroz, "[Identification of bitmap compression history: JPEG detection and quantizer estimation](http://queiroz.divp.org/papers/quant_estimation_jpeg.pdf)," IEEE Trans. on Image Processing, Vol. 12, pp. 230-235, Feb. 2003.
* R. Neelamani, R. de Queiroz, Z. Fan, S. Dash and R. Baraniuk, "[JPEG compression history estimation for color images](http://queiroz.divp.org/papers/neelsh-journal.pdf)," IEEE Trans. on Image Processing, Vol. 15, No 6, pp. 1365-1378, June 2006.
* R. Neelamani, R. Baraniuk, and R. de Queiroz, "[Compression color space estimation of JPEG images using lattice basis reduction](http://queiroz.divp.org/papers/icip01lattice.pdf)," Proc. IEEE Intl. Conf. on Image Processing, ICIP, Greece, pp. 890-893, 2001.