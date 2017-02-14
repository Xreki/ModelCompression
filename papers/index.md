## Deep Compression

- Learning both Weights and Connections for Efficient Neural Networks [[NIPS 2015](https://arxiv.org/abs/1506.02626)]
	- Song Han, Jeff Pool, John Tran, William J. Dally
	- 2015-06-08 (v1), 2015-10-30 (v3)
	- [detail](deep-compression/test.txt)
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
- QuickNet: Maximizing Efficiency and Efficacy in Deep Architectures [[arxiv](https://arxiv.org/abs/1701.02291)]
    - Tapabrata Ghosh
    - 2017-01-09 (v1), 2017-01-12 (v2)
<<<<<<< .mine
- The Incredible Shrinking Neural Network: New Prespectives on Learning Representations Through The Lens of Pruning [[arxiv](https://arxiv.org/abs/1701.04465)]
	- Nikolas Wolfe, Aditya Sharma, Lukas Drude, ...
	- 2017-01-16 (v1)







=======
- Pruning Convolutional Neural Networks for Resource Efficient Inference [[ICLR 2017](https://openreview.net/pdf?id=SJGCiw5gl)]
    - Pavlo Molchanov, Stephen Tyree, Tero Karras, Timo Aila, Jan Kautz
    - 2016-11-05
- Faster CNNs with Direct Sparse Convolutions and Guided Pruning [[ICLR 2017](https://openreview.net/pdf?id=rJPcZ3txx)]
    - Jongsoo Park, Sheng Li, Wei Wen, Ping Tak Peter Tang, Hai Li, Yiran Chen, Pradeep Dubey
    - 2016-11-04
    - [[Homepage of Jongsoo Park](https://sites.google.com/site/jongsoopark/home)]
- Towards the Limit of Network Quantization [[ICLR 2017](https://openreview.net/pdf?id=rJ8uNptgl)]
    - Yoojin Choi, Mostafa El-Khamy, Jungwon Lee
    - 2016-11-04
>>>>>>> .theirs
- Some slices
	- [Deep Compression and EIE](https://web.stanford.edu/class/ee380/Abstracts/160106-slides.pdf)
- [Home of Song Han](https://stanford.edu/~songhan/)


## Quantilization

### Fixed-precision
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
<<<<<<< .mine
- Two-Bit Networks for Deep Learning on Resource-Constrained Embedded Devices [[arxiv](https://arxiv.org/abs/1701.00485)]
	- Wenjia Meng, Zonghua Gu, Ming Zhang, ...
	- 2017-01-02 (v1), 2017-01-04 (v2)
=======
- Incremental Network Quantization: Towards Lossless CNNs with Low-precision Weights [[ICLR 2017](https://openreview.net/pdf?id=HyQJ-mclg)]
    - Aojun Zhou, Anbang Yao, Yiwen Guo, Lin Xu, Yurong Chen
    - 2016-11-04
>>>>>>> .theirs

## Distilling
- Distilling the Knowledge in a Neural Network [[NIPS 2014 Deep Learning Workshop](Distilling the Knowledge in a Neural Network)]
	- Geoffrey Hinton, Oriol Vinyals, Jeff Dean
	- 2015-03-09 (v1)
- Face model compression by distilling knowledge from neurons [[AAAI 2016](http://www.aaai.org/ocs/index.php/AAAI/AAAI16/paper/download/11977/12130)]
	- Ping Luo, Zhenyao Zhu, Ziwei Liu

## Decomposition
- CP-decomposition with Tensor Power Method for Convolutional Neural Networks Compression [[BigComp 2017](https://arxiv.org/abs/1701.07148)]
	- Marcella Astrid, Seung-lk Lee
	- 2017-01-25 (v1)

## Others
- Dynamic Network Surgery for Efficient DNNS [Intel] [[NIPS 2016](https://arxiv.org/abs/1608.04493)]
	- Yiwen Guo, Anbang Yao, Yurong Chen
	- 2016-08-16 (v1), 2016-11-10 (v2)
<<<<<<< .mine
- Varitional Dropout Sparsifies Deep Neural Networks [[arxiv](https://arxiv.org/abs/1701.05369)]
	- Dmitry Molchanov, Arsenii Ashukha, Dmitry Vetrov
	- 2017-01-19 (v1)
- Compression of Deep Neural Networks for Image Instance Retrieval [[DCC 2017](https://arxiv.org/abs/1701.04923)]
	- Vijay Chandrasekhar, Jie Lin, Qianli Liao, ...
	- 2017-01-18




=======
- DeepRebirth: A General Approach for Accelerating Deep Neural Network Execution on Mobile Devices [[ICLR 2017](https://openreview.net/pdf?id=SkwSJ99ex)]
    - Dawei Li, Xiaolong Wang, Deguang Kong, Mooi Choo Chuah
    - 2016-11-05
- Tartan: Accelerating Fully-Connected and Convolutional Layers in Deep Learning Networks by Exploiting Numerical Precision Variability [[ICLR 2017](https://openreview.net/pdf?id=Hy-lMNqex)]
    - Alberto Delmás Lascorz, Sayeh Sharify, Patrick Judd, Andreas Moshovos
    - 2016-11-05
- FastText.zip: Compressing text classification models [[ICLR 2017](https://openreview.net/pdf?id=SJc1hL5ee)]
    - Armand Joulin, Edouard Grave, Piotr Bojanowski, Matthijs Douze, Herve Jegou, Tomas Mikolov
    - 2016-11-05
 
>>>>>>> .theirs
