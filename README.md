# Dual Residual Networks  
By Xing Liu<sup>1</sup>, [Suganuma Masanori](https://scholar.google.co.jp/citations?user=NpWGfwgAAAAJ&hl=ja)<sup>1,2</sup>, [Zhun Sun](https://scholar.google.co.jp/citations?user=Y-3iZ9EAAAAJ&hl=en)<sup>2</sup>, [Takayuki Okatani](https://scholar.google.com/citations?user=gn780jcAAAAJ&hl=en)<sup>1,2</sup>


Tohoku University<sup>1</sup>, RIKEN Center for AIP<sup>2</sup>

[link to the paper](https://arxiv.org/pdf/1903.08817.pdf)

## Table of Contents
1) Abstract

2) Citation

3) Numerical Results

4) Models 

5) Datasets 

6) Test

7) Train (coming soon)

8) Visual Results


## Abstract
In this paper, we study design of deep neural networks for tasks of image restoration. We propose a novel style of residual connections dubbed “dual residual connection”, which exploits the potential of paired operations, e.g., upand down-sampling or convolution with large- and smallsize kernels. We design a modular block implementing this connection style; it is equipped with two containers to which arbitrary paired operations are inserted. Adopting the “unraveled” view of the residual networks proposed by Veit et al., we point out that a stack of the proposed modular blocks allows the first operation in a block interact with the second operation in any subsequent blocks. Specifying the two operations in each of the stacked blocks, we build a complete network for each individual task of image restoration. We experimentally evaluate the proposed approach on five image restoration tasks using nine datasets. The results show that the proposed networks with properly chosen paired operations outperform previous methods on almost all of the tasks and datasets.


## Citation
```
@inproceedings{DuRN_cvpr19,
title={Dual Residual Networks Leveraging the Potential of Paired Operations for Image Restoration},
author={Liu, Xing and Suganuma, Masanori and Sun, Zhun and Okatani, Takayuki},
booktitle={arXiv preprint arXiv:1903.08817},
year={2019},
}
```

## Numerical results
Please find them in the <code>test/results_confirmed.txt</code> file.

## Models
Please find them
[here](https://drive.google.com/file/d/1Fi6B3Lm_8afu_Ak8LxGihXJTd2XGx9Y2/view?usp=sharing).

## Datasets
### Gaussian noise removal
[BSD500-gray](https://drive.google.com/file/d/1-Q0tCxzisHm7m_qMJfekOy4-oGzfIocj/view?usp=sharing) (used in our paper)\
If you also want the original BSD500, click [here](https://www2.eecs.berkeley.edu/Research/Projects/CS/vision/bsds/).

### Real-world noise removal
[RealNoise-HKPolyU](https://github.com/csjunxu/PolyU-Real-World-Noisy-Images-Dataset)\
Also check this paper ([arXiv](https://arxiv.org/pdf/1804.02603.pdf)) for more info. for the dataset.

[RealNoise-test](https://drive.google.com/file/d/1jopTnkHjukCHQ5Og4gwwEdvBQxGV7Bhf/view?usp=sharing) \
This is the test-set used in our paper. We generated it by random cropping on 10 HR samples.


## Visual results
### Gaussian noise removal
![](https://github.com/liu-vis/DualResidualNetworks/blob/master/Figs/gaussian_noise.png)

### Real-world noise removal
![](https://github.com/liu-vis/DualResidualNetworks/blob/master/Figs/real_noise.png)

### Motion blur removal - 1
![](https://github.com/liu-vis/DualResidualNetworks/blob/master/Figs/supp_blur_mix.png)

### Motion blur removal - 2
Some examples for object detection
![](https://github.com/liu-vis/DualResidualNetworks/blob/master/Figs/supp_blur_detect.png)

### Haze removal - 1
The images are taken by iphone 6 plus
![](https://github.com/liu-vis/DualResidualNetworks/blob/master/Figs/supp_haze_iphone.png)

### Haze removal - 2
![](https://github.com/liu-vis/DualResidualNetworks/blob/master/Figs/supp_haze_real_4ver.png)

### Haze removal - 3
Compare inside-feature maps with transmission map
![](https://github.com/liu-vis/DualResidualNetworks/blob/master/Figs/supp_transmission.png)

### Raindrop removal
![](https://github.com/liu-vis/DualResidualNetworks/blob/master/Figs/supp_raindrop.png)

### Rain-streak removal
![](https://github.com/liu-vis/DualResidualNetworks/blob/master/Figs/supp_rain_syn.png)


