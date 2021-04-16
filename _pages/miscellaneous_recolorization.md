---
title: "Recolorization"
author_profile: true
layout: single
sidebar:
  nav: "projs"
classes: wide
permalink: /miscellaneous-recolorization/
---

<p style="text-align:center;">
  <img src="https://github.com/DiogoCaetanoGarcia/minimal-mistakes/raw/master/assets/images/recolorization1.png"><br>
  <img src="https://github.com/DiogoCaetanoGarcia/minimal-mistakes/raw/master/assets/images/recolorization2.png"><br>
  <img src="https://github.com/DiogoCaetanoGarcia/minimal-mistakes/raw/master/assets/images/recolorization3.png"><br>
</p>

We introduced the concept of reversible conversion of color images to gray ones, wherein colors are mapped to textures and from the textures the receiver can recover the colors. This was done using the wavelet transform (or other subband transform) and replacing high-frequency subbands by the down-sampled chrominance planes. The idea is to print a color image with a black and white printer and, then, at a later time, to scan the document and recover colors. We developed simpler and more robust schemes, using the discrete wavelet transform and multiple subbands as well. 

### Publications

* R. L. de Queiroz, "[Reversible color-to-gray mapping using subband domain texturization](http://queiroz.divp.org/papers/colortobw-subbands-prl.pdf)," Pattern Recognition Letters, Vol. 31, No. 4, pp. 269-276, Mar. 2010.
* R. L. de Queiroz and K. Braun, "[Color to gray and back: color embedding into textured gray images](http://queiroz.divp.org/papers/color-to-bw.pdf)," IEEE Trans. on Image Processing, Vol. 15, No 6, pp. 1464-1470, June 2006.