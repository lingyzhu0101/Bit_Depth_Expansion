# [MMSP'24] Bit_Depth_Expansion
Official Pytorch implementation of **Unrolled Decomposed Unpaired Learning for Controllable Low-Light Video Enhancement**.

[Lingyu Zhu](https://scholar.google.com/citations?user=IhyTEDkAAAAJ&hl=zh-CN),
[Wenhan Yang](https://scholar.google.com/citations?user=S8nAnakAAAAJ&hl=zh-CN),
[Baoliang Chen](https://scholar.google.com/citations?user=w_WL27oAAAAJ&hl=zh-CN),
[Hanwei Zhu](https://scholar.google.com/citations?user=-52izjkAAAAJ&hl=zh-CN),
[Zhangkai Ni](https://scholar.google.com/citations?hl=zh-CN&user=68IcrE4AAAAJ),
[Qi Mao](https://scholar.google.com/citations?hl=zh-CN&user=VTQZF6EAAAAJ),
[Shiqi Wang](https://scholar.google.com/citations?user=Pr7s2VUAAAAJ&hl=zh-CN)


[[`Arxiv`](http://arxiv.org/abs/2408.12316)] [[`Poster`](src/figures/ECCV_poster.png)] [[`Video`](https://www.youtube.com/watch?v=gn_IB1-FEY8&t=2s)] [[`Invited_Talk`](src/figures/Presentation_in_NTU.pdf)]

## Overview
<p align="left">
<img src="src/figures/framework.png" width=80% height=80% 
class="center">
</p>

Diffusion-based generative models have achieved
remarkable success across a variety of applications. However, the
potential application for bit-depth expansion has not been exten-
sively studied. This paper introduces a wavelet-based diffusion
model for the bit-depth expansion task. In this method, the image
is first decomposed into low and high-frequency components via
wavelet transformation. This decomposition allows for targeted
processing by specialized modules and reduces computational
complexity by lowering the image resolution. The low-frequency
component is processed in both the forward diffusion and reverse
denoising stages. Meanwhile, the high-frequency components are
filtered by the High Frequency Denoising Filter (HFDF) to
eliminate noise and artifacts. Finally, the low and high-frequency
components are recombined into a predicted high-bit-depth
image through inverse wavelet transformation. Experimental
results demonstrate the superiority of the proposed method
in producing perceptually compelling outputs that outperform
previous methods

## Qualitative Performance
<p align="left">
<img src="src/figures/main_performance_qualitative.png" width=80% height=80% 
class="center">
</p>


## Quantitative Performance
<p align="left">
<img src="src/figures/main_performance_quantitative.png.png" width=80% height=80% 
class="center">
</p>


## TODO List
This repository is still under active construction:
- [x] Release training and testing codes
- [ ] Release pretrained models
- [ ] Clean the code
