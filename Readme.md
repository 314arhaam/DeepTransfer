# :computer: :art: DeepTransfer: Another Style Transfer Project
Based on the work of [Gatys et. al.](https://openaccess.thecvf.com/content_cvpr_2016/papers/Gatys_Image_Style_Transfer_CVPR_2016_paper.pdf)

## Introduction
Style Transfer, is the process of creating an image "C", with the same "content" of an image "A", with the style of an image "B". In other words, reproducing the [**Mona Lisa**](https://en.wikipedia.org/wiki/Mona_Lisa) painting, with the style of [**The Starry Night**](https://en.wikipedia.org/wiki/The_Starry_Night).  
## Methodology
In lyman terms, at first, a pretriend image classifier (e.g. VGG-19) is used to extract different convo-layers of an image. Early layers, represent the content of an image and deeper layers, represent the style. In case of "Mona Lisa", the early layers, represent the woman, and the deeper layers, represent the color scheme and stroke.  
Early layers of image A and deeper layers of image B will be extracted. The same process will be done on the result image. Then, by an optimization process, the difference between early and deeper layers of the result image, and the respective layers of images A and B, will be minimized.  
## Results
That's how it works:  
<p align="center">
  <img src="https://github.com/314arhaam/DeepTransfer/blob/master/results/style-transfer-diagram.png" height=400/>
</p>
  
## BibTex
Bibliography of the reference works.  
```
@InProceedings{Gatys_2016_CVPR,
author = {Gatys, Leon A. and Ecker, Alexander S. and Bethge, Matthias},
title = {Image Style Transfer Using Convolutional Neural Networks},
booktitle = {Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition (CVPR)},
month = {June},
year = {2016}
```
