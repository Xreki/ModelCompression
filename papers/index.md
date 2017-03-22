# Deep Compression

- Learning both Weights and Connections for Efficient Neural Networks [[NIPS 2015](https://arxiv.org/abs/1506.02626)] [[notes](pruning/deep-compression/test.txt)]
	- Song Han, Jeff Pool, John Tran, William J. Dally
	- 2015-06-08 (v1), 2015-10-30 (v3)
- Deep Compression: Compressing Deep Neural Networks with Pruning, Trained Quantization and Huffman Coding [[ICLR 2016](https://arxiv.org/abs/1510.00149)]
	- Song Han, Huizi Mao, William J. Dally
	- 2015-10-01 (v1), 2016-02-15 (v5)
- EIE: Efficient Inference Engine on Compressed Deep Neural Network [[ISCA 2016](https://arxiv.org/abs/1602.01528)]
	- Song Han, Xingyu Liu, Huizi Mao, ...
	- 2016-02-04 (v1), 2016-05-03 (v2)
- ESE: Efficient Speech Recognition Engine with Compressed LSTM on FPGA [[FPGA 2017](https://arxiv.org/abs/1612.00694)]
	- Song Han, Junlong Kang, Huizi Mao, ...
	- 2016-12-01 (v1)
- DSD: Regularizing Deep Neural Networks with Dense-Sparse-Dense Training Flow [[arxiv](https://arxiv.org/abs/1607.04381)]
	- Song Han, Jeff Pool, Sharan Narang, ...
	- 2016-07-15 (v1)
- SqueezeNet: AlexNet-level accuracy with 50x fewer parameters and <0.5MB model size [[arxiv](https://arxiv.org/abs/1602.07360)]
	- Forrest N. landola, Song Han, Matthew W. Moskewicz, ...
	- 2016-02-24 (v1), 2016-11-04 (v4)
- Some slices
	- [Deep Compression and EIE](https://web.stanford.edu/class/ee380/Abstracts/160106-slides.pdf)
- [Home of Song Han](https://stanford.edu/~songhan/)

# Sparsity
- Sparse convolutional neural network [[CVPR 2015](http://www.cv-foundation.org/openaccess/content_cvpr_2015/papers/Liu_Sparse_Convolutional_Neural_2015_CVPR_paper.pdf)]
	- sparsity regularization, l1-norm
- Learning Structured Sparsity in Deep Neural Network [[NIPS 2016](https://arxiv.org/abs/1608.03665)] [[notes](pruning/sparsity/Learning_Structured_Sparsity_in_Deep_Neural_Networks.md)] [[github](https://github.com/wenwei202/caffe/tree/scnn)]
	- Wei Wen, Chupeng Wu, Yandan Wang, ...
	- 2016-08-12 (v1), 2016-10-18 (v4)
	- group-wise sparsity patterns; Structured Sparsity Learning (SSL), group Lasso regularization; 5.1x and 3.1x speedups of convolutional layer computation of AlexNet against CPU and GPU
- Faster CNNs with Direct Sparse Convolutions and Guided Pruning [[ICLR 2017](https://openreview.net/pdf?id=rJPcZ3txx)] [[notes](pruning/sparsity/Faster_CNNs_with_Direct_Sparse_Convolutions_and_Guided_Pruning.md)] [[github](https://github.com/IntelLabs/SkimCaffe)]
    - Jongsoo Park, Sheng Li, Wei Wen, Ping Tak Peter Tang, Hai Li, Yiran Chen, Pradeep Dubey
    - 2016-11-04
    - Pruning CNNs; AlexNet: 7.3x on Intel Atom; 3.4x on Intel Xeon; 3.1x on Knights Landing; non-zero proportion 0.09; no accuracy drop
    - [Homepage of Jongsoo Park](https://sites.google.com/site/jongsoopark/home)
- The Power of Sparsity in Convolutional Neural Networks [Google][[arxiv](https://arxiv.org/pdf/1702.06257)]
    - Soravit Changpinyo, Mark Sandler, Andrey Zhmoginov
    - 2017-02-21
- Dynamic Network Surgery for Efficient DNNs [Intel] [[NIPS 2016](https://arxiv.org/abs/1608.04493)] [[notes](pruning/others/Dynamic_Network_Surgery_for_Efficient_DNNs.md)] [[github](https://github.com/yiwenguo/Dynamic-Network-Surgery)]
	- Yiwen Guo, Anbang Yao, Yurong Chen
	- 2016-08-16 (v1), 2016-11-10 (v2)
	- compress the number of parameters: LeNet-5, 108x; AlexNet, 17.7x; without any accuracy loss
- Pruning Convolutional Neural Networks for Resource Efficient Inference [[ICLR 2017](https://openreview.net/pdf?id=SJGCiw5gl)]
    - Pavlo Molchanov, Stephen Tyree, Tero Karras, Timo Aila, Jan Kautz
    - 2016-11-05
- The Incredible Shrinking Neural Network: New Prespectives on Learning Representations Through The Lens of Pruning [[arxiv](https://arxiv.org/abs/1701.04465)]
	- Nikolas Wolfe, Aditya Sharma, Lukas Drude, ...
	- 2017-01-16 (v1)
- Enabling Sparse Winograd Convolution by Native Pruning [[arxiv](https://arxiv.org/pdf/1702.08597.pdf)]
    - Sheng Li, Jongsoo Park, Ping Tak Peter Tang
    - 2017-03-01

# Quantilization

### Fixed Precision
- Improving the speed of neural networks on CPUs [Google] [[NIPS 2011's workshop](https://static.googleusercontent.com/media/research.google.com/zh-CN//pubs/archive/37631.pdf)]
	- Vincent Vanhoucke, Andrew Senior, Mark Z. Mao
- On the efficient representation and execution of deep acoustic models [Google] [[Interspeech 2016](https://arxiv.org/abs/1607.04683)]
	- Raziel Alvarez, Rohit Prabhavalkar, Anton Bakhtin
	- 2016-07-15 (v1), 2016-12-17 (v2)
	- How to Quantize Neural Networks with TensorFlow [[English](https://petewarden.com/2016/05/03/how-to-quantize-neural-networks-with-tensorflow/)] [[Chinese](http://fjdu.github.io/machine/learning/2016/07/07/quantize-neural-networks-with-tensorflow.html)]
- Fast, Compact, and High Quality LSTM-RNN Based Statistical Parametric Speech Synthesizers for Mobile Devices [Google] [[Interspeech 2016](https://arxiv.org/abs/1606.06061)]
	- Heiga Zen, Yannis Agiomyrgiannakis, Niels Egberts, ...
	- 2016-06-20 (v1), 2016-06-22 (v2)
- On The Compression Of Recurrent Neural Networks With An Application To LVCSR Acoustic Modeling For Embedded Speech Recognition [Google] [[ICASSP 2016](https://arxiv.org/pdf/1603.08042.pdf)]
	- Rohit Prabhanalkar, Ouais Alsharif, Autoine Bruguier


### Q-CNN
- Quantized Convolutional Neural Networks for Mobile Devices [[CVPR 2016](https://arxiv.org/abs/1512.06473)] [[codes](https://github.com/jiaxiang-wu/quantized-cnn)]
	- Jiaxiang Wu, Cong Leng, Yuhang Wang
	- 2015-12-21 (v1), 2016-05-16 (v3)

### Low Precision
- Deep Learning with Limited Numerical Precision [IBM] [[arxiv](https://arxiv.org/abs/1502.02551)]
	- Suyog Gupta, Ankur Agrawal, Kailash Gopalakrishnan, Pritish Narayanan
	- 2015-02-09 (v1)
- Training deep neural networks with low precision multiplications [[ICLR 2015](https://arxiv.org/abs/1412.7024)]
	- Matthieu Courbariaux, Yoshua Bengio, Jean-Pieirre David
	- 2014-12-22 (v1), 2015-04-03 (v5)
- BinaryConnect: Training Deep Neural Networks with binary weights during propagations [[NIPS 2015](https://arxiv.org/abs/1511.00363)]
	- Matthieu Courbariaux, Yoshua Bengio, Jean-Pierre David
	- 2015-11-02 (v1), 2016-04-18 (v3)
- XOR-Net: ImageNet Classification Using Binary Convolutional Neural Networks [[arxiv](https://arxiv.org/abs/1603.05279)]
	- Mohammad Rastegari, Vicente Ordonez, Joseph Redmon, ...
	- 2016-05-16 (v1), 2016-08-02 (v4)
- Deep Learning with low Precision by Half-wave Gaussian Quantization [[arxiv](https://arxiv.org/abs/1702.00953)]
	- Zhaowei Cai, Xiaodong He, Jian Sun, ...
	- 2017-02-03 (v1)
- Incremental Network Quantization: Towards Lossless CNNs with Low-precision Weights [[ICLR 2017](https://openreview.net/pdf?id=HyQJ-mclg)]
    - Aojun Zhou, Anbang Yao, Yiwen Guo, Lin Xu, Yurong Chen
    - 2016-11-04
- Two-Bit Networks for Deep Learning on Resource-Constrained Embedded Devices [[arxiv](https://arxiv.org/abs/1701.00485)]
	- Wenjia Meng, Zonghua Gu, Ming Zhang, ...
	- 2017-01-02 (v1), 2017-01-04 (v2)
- Low-Precision Batch-Normalized Activations [[arxiv](https://arxiv.org/pdf/1702.08231.pdf)]
    - Benjamin Graham
    - 2017-02-27
- Fixed-point optimization of deep neural networks with adaptive step size retraining [[arxiv](https://arxiv.org/pdf/1702.08171.pdf)]
    - Sungho Shin, Yoonho Boo, Wonyong Sung
    - 2017-02-27
- Trained Ternary Quantization [[arxiv](https://arxiv.org/pdf/1612.01064.pdf)]
    - Chenzhuo Zhu, Song Han, Huizi Mao, William J. Dally
    - 2017-02-23
    
### Others
- Towards the Limit of Network Quantization [[ICLR 2017](https://openreview.net/pdf?id=rJ8uNptgl)]
    - Yoojin Choi, Mostafa El-Khamy, Jungwon Lee
    - 2016-11-04


# Distilling
- Distilling the Knowledge in a Neural Network [[NIPS 2014 Deep Learning Workshop](https://arxiv.org/abs/1503.02531)]
	- Geoffrey Hinton, Oriol Vinyals, Jeff Dean
	- 2015-03-09 (v1)
- Face model compression by distilling knowledge from neurons [[AAAI 2016](http://www.aaai.org/ocs/index.php/AAAI/AAAI16/paper/download/11977/12130)]
	- Ping Luo, Zhenyao Zhu, Ziwei Liu

# Decomposition
- Speeding up Convolutional Neural Networks Using Fine-tuned CP-Decompositon [[ICLR 2015](https://arxiv.org/abs/1412.6553)]
	- Vadim Lebedev, Victor Lempitsky
	- 2014-12-19 (v1), 2015-04-24 (v3)
- CP-decomposition with Tensor Power Method for Convolutional Neural Networks Compression [[BigComp 2017](https://arxiv.org/abs/1701.07148)]
	- Marcella Astrid, Seung-lk Lee
	- 2017-01-25 (v1)
- Compression of Deep Convolutional Neural Networks for Fast and Low Power Mobile Applications [[arixv](https://arxiv.org/abs/1511.06530)]
    - Yong-Deok Kim, Eunhyeok Park, Sungjoo Yoo, Taelim Choi, Lu Yang, Dongjun Shin
    - 2016-02-24 (v2)

# Others
- DeepRebirth: A General Approach for Accelerating Deep Neural Network Execution on Mobile Devices [[ICLR 2017](https://openreview.net/pdf?id=SkwSJ99ex)]
    - Dawei Li, Xiaolong Wang, Deguang Kong, Mooi Choo Chuah
    - 2016-11-05
- Tartan: Accelerating Fully-Connected and Convolutional Layers in Deep Learning Networks by Exploiting Numerical Precision Variability [[ICLR 2017](https://openreview.net/pdf?id=Hy-lMNqex)]
    - Alberto Delmás Lascorz, Sayeh Sharify, Patrick Judd, Andreas Moshovos
    - 2016-11-05
- FastText.zip: Compressing text classification models [[ICLR 2017](https://openreview.net/pdf?id=SJc1hL5ee)]
    - Armand Joulin, Edouard Grave, Piotr Bojanowski, Matthijs Douze, Herve Jegou, Tomas Mikolov
    - 2016-11-05
- Varitional Dropout Sparsifies Deep Neural Networks [[arxiv](https://arxiv.org/abs/1701.05369)]
	- Dmitry Molchanov, Arsenii Ashukha, Dmitry Vetrov
	- 2017-01-19 (v1)
- Compression of Deep Neural Networks for Image Instance Retrieval [[DCC 2017](https://arxiv.org/abs/1701.04923)]
	- Vijay Chandrasekhar, Jie Lin, Qianli Liao, ...
- LightRNN: Memory and Computation-Efficient Recurrent Neural Networks [Microsoft] [[NIPS 2016](https://arxiv.org/abs/1610.09893)] [[blog](http://www.msra.cn/zh-cn/news/blogs/2016/12/lightrnn-20161228.aspx)]
	- Xiang Li, Tao Qin, Jian Yang, ...
	- 2016-10-31 (v1)
- Soft Weight-Sharing for Neural Network Compression [[ICLR 2017](https://arxiv.org/pdf/1702.04008)]
    - Karen Ullrich, Edward Meeds, Max Welling
- QuickNet: Maximizing Efficiency and Efficacy in Deep Architectures [[arxiv](https://arxiv.org/abs/1701.02291)]
    - Tapabrata Ghosh
    - 2017-01-09 (v1), 2017-01-12 (v2)
- ShaResNet: Reducing Residual Network Parameter Number by Sharing Weights [[arxiv](https://arxiv.org/pdf/1702.08782.pdf)]
    - Alexandre Boulch
    - 2017-03-01


