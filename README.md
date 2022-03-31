# SNN-learning-methods-papers
该仓库主要收录了顶会中SNN领域的一些论文，论文内容与代理梯度(sg)和ANN-SNN转换相关。

目录
[rookie](##rookie)


##rookie

## must-read sg papers
- Surrogate Gradient Learning in Spiking Neural Networks. (Mostafa) [Link](https://arxiv.org/pdf/1901.09948.pdf)
    > describe: Rate-based sg. SNNs like RNNs

- Spatio-temporal backpropagation for training high-performance spiking neural networks. (WuYujie) [Link](https://www.frontiersin.org/articles/10.3389/fnins.2018.00331/full)
    > describe: Rate-based sg. 利用BPTT训练SNN

## must-read ann-snn works
- Conversion of continuous-valued deep networks to efficient event-driven networks for image classification. (Rueckauer) [Link](https://www.frontiersin.org/articles/10.3389/fnins.2017.00682/full)
    > describe: Rate-based conversion. 

## ICML
### 2020
- Rmp-snn: Residual membrane potential neuron for enabling deeper high-accuracy and low-latency spiking neural network. (HanBing) [Link](https://openaccess.thecvf.com/content_CVPR_2020/papers/Han_RMP-SNN_Residual_Membrane_Potential_Neuron_for_Enabling_Deeper_High-Accuracy_and_CVPR_2020_paper.pdf)
    > describe: Rate-based conversion. 对soft-reset分析透彻。利用soft-reset第一次将conversion做在大规模网络上。


### 2021
- A free lunch from ANN: Towards efficient, accurate spiking neural networks calibration. (Gushi) [Link](http://proceedings.mlr.press/v139/li21d/li21d.pdf)
    > describe: Rate-based conversion. 该论文在ICLR2021工作的基础上，加入了逐层缩小误差的方法。效果非常好

## ICLR
### 2021
- Optimal conversion of conventional artificial neural networks to spiking neural networks. (Gushi) [Link](https://arxiv.org/pdf/2103.00476.pdf)
    > describe: Rate-based conversion. 该论文系统分析了转换的flooring error。conversation必读论文。

### 2022
- Temporal Efficient Training of Spiking Neural Network via Gradient Re-weighting. (Gushi) [Link](https://arxiv.org/pdf/2202.11946.pdf)
    > describe: Rate-based SG. 该论文对loss的计算进行了调整。

- Optimal ANN-SNN Conversion for High-accuracy and Ultra-low-latency Spiking Neural Networks. (YuZhaofei) [Link](https://openreview.net/pdf?id=7B3IJMM1k_M)
    > describe: Rate-based conversion. 该论文系统分析了三种转换误差，提出将QNN转SNN。推荐读。


## NeurIPS
### 2021
- Differentiable Spike: Rethinking Gradient-Descent for Training Spiking Neural Networks. (Gushi) [Link](https://proceedings.neurips.cc/paper/2021/file/c4ca4238a0b923820dcc509a6f75849b-Paper.pdf)
    > describe: Rate-based SG. 


## IJCAI
### 2021
- Optimal ann-snn conversion for fast and accurate inference in deep spiking neural networks. (YuZhaofei) [Link](https://arxiv.org/pdf/2105.11654.pdf)
    > describe: Rate-based conversion. 通过BP的方式得到最优的正则化参数。


## AAAI
### 2021

### 2022
- Optimized Potential Initialization for Low-latency Spiking Neural Networks. (YuZhaofei) [Link](https://www.aaai.org/AAAI22Papers/AAAI-3681.BuT.pdf)
    > describe: Rate-based conversion. 该论文提出将神经元初始膜电压设为二分之阈值来缩小flooring error，简单好用。
