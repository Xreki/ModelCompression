## Abstract
1. While pruning the fully connected layers reduces a CNN’s size considerably, it
does not improve inference speed noticeably as the compute heavy parts lie in
convolutions. Pruning CNNs in a way that increase inference speed often imposes
specific sparsity structures, thus limiting the achievable sparsity levels.
2. pruning CNNs: simultaneously size economy + speed improvement
	- an efficient general **sparse-with-dense matrix multiplication** implementation that is applicable to convolution of feature maps with **kernels of arbitrary sparsity patterns**.
	- a performance model that predicts sweet spots of sparsity levels for different layers and on different computer architectures.
	- **3.1–7.3x convolution speedups over dense convolution in AlexNet**, on Intel Atom, Xeon, and Xeon Phi processors, spanning the spectrum from mobile devices to supercomputers.

## 摘要
1. 裁剪fc能很大程度上减少cnn的大小，但是对cnn预测的速度没有太大的影响，因为cnn速度的瓶颈在于卷积层。以某种能增加预测速度的方式裁剪卷积层，通常会引起特殊的稀疏结构，因此会影响稀疏的程度。
2. 裁剪CNN：减小大小 + 加快速度
	- 一种高效通用的sparse-with-dense矩阵乘实现，它可作用于任意稀疏模式的feature kernel的卷积
	- 一个性能模型，可以在不同架构上预测不同网络层中，不同稀疏程度的收益
	- 相比稠密的AlexNet模型，带来**3.1-7.3x的加速**，在Intel Atom（手机）、Xeon（CPU服务器）、Xeon Phi processors（众核服务器）上

## 主要贡献
- a highly efficient direct sparse convolution design formulated as sparse-matrix-dense-matrix multiplication with the dense matrix columns generated on-the -fly from a signle column vector
- 直接稀疏卷积的设计，称之为sparse-matrix-dense-matrix multiplication，其中稠密矩阵的列是计算的时候从一个列向量生成的
- a performance model to elucidate when and how best to use sparse convolutions on different computer architectures and at different CNN layers
- 一个性能模型，可以针对不同的架构、不同的模型给出什么时候、怎么样最好地使用稀疏卷积。
	- 基于roofline model。
	- 模型显示，即使70%的稀疏化，预测也能得到加速。
	- 给出预测能够加速的稀疏化比例的上限、下限
- new pruning algorithm——Guided Sparsity Learning (GSL)
	- can adjust sparsity targets precisely at different layers so as to maximize inference speed, best preserve accuracy, and minimize a network's size
- an optimized sparse convolution implementation [[github](https://github.com/IntelLabs/SkimCaffe)]
	- AlexNet: 7.3x on Intel Atom; 3.4x on Intel Xeon; 3.1x on Knights Landing; no accuracy drop;

## Direct Sparse Convolution


## Performance Model


## Guided Sparsity Learning (GSL) pruning algorithm


## Experiments' Result

- Xeon E5-2697 v4 (BDW): 3.4x加速，非零元比例x=0.09
- Xeon Phi 7250 (KNL): 3.1x加速，非零元比例x=0.09
- Intel C2750 (Atom): 7.3x加速，非零元比例x=0.09

