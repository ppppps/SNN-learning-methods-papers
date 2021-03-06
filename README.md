# SNN-learning-methods-papers
该仓库主要收录了顶会中SNN领域的一些论文，论文内容与代理梯度(sg)和ANN-SNN转换相关。

# 目录
* [入门](#入门)
* [进阶](#进阶)

# 入门
- 脉冲神经网络研究进展综述 (WuYujie)
[Link](https://kns.cnki.net/kcms/detail/detail.aspx?dbcode=CJFD&dbname=CJFDLAST2021&filename=KZYC202101001&uniplatform=NZKPT&v=OKAgri6ShmMthMiPGj5fmuHE2CjFOD7VktWGScxfWQGOrcewzwu16QQNNVybMLTM)
    > describe: 目前最好的SNN中文综述，入门SNN看这一篇足以。

# 进阶

## must-read sg papers
- Surrogate Gradient Learning in Spiking Neural Networks. (Mostafa) [Link](https://arxiv.org/pdf/1901.09948.pdf)
    > describe: Rate-based sg. SNNs like RNNs

- Spatio-temporal backpropagation for training high-performance spiking neural networks. (WuYujie) [Link](https://www.frontiersin.org/articles/10.3389/fnins.2018.00331/full)
    > describe: Rate-based sg. 利用BPTT训练SNN

## must-read ann-snn works
- Conversion of continuous-valued deep networks to efficient event-driven networks for image classification. (Rueckauer) [Link](https://www.frontiersin.org/articles/10.3389/fnins.2017.00682/full)
    > describe: Rate-based conversion. 

- Fast-Classifying, High-Accuracy Spiking Deep Networks Through Weight and Threshold Balancing. (LiuShichi) [Link](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.721.2413&rep=rep1&type=pdf)
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
    
- Deep Residual Learning in Spiking Neural Networks. (YuZhaofei) [Link](https://arxiv.org/pdf/2102.04159.pdf)
    > describe: Rate-based Method. 针对SNN使用ResNet结构时无法实现identity mapping的问题，将IF神经元放入block中，实现identity mapping。 

## IJCAI
### 2021
- Optimal ann-snn conversion for fast and accurate inference in deep spiking neural networks. (YuZhaofei) [Link](https://arxiv.org/pdf/2105.11654.pdf)
    > describe: Rate-based conversion. 通过BP的方式得到最优的正则化参数。


## AAAI
### 2019
- Direct Training for Spiking Neural Networks: Faster, Larger, Better. (WuYujie) [Link](https://arxiv.org/pdf/1809.05793.pdf)
    > describe: Rate-based SG. 提出NeuronNorm。是STBP的后续工作，推荐读。

### 2021
- Going Deeper With Directly-Trained Larger Spiking Neural Networks. (WuYujie) [Link](https://arxiv.org/pdf/2011.05280.pdf)
    > describe: Rate-based SG. 提出tdBN。是STBP的后续工作，推荐读。

### 2022
- Optimized Potential Initialization for Low-latency Spiking Neural Networks. (YuZhaofei) [Link](https://www.aaai.org/AAAI22Papers/AAAI-3681.BuT.pdf)
    > describe: Rate-based conversion. 该论文提出将神经元初始膜电压设为二分之阈值来缩小flooring error，简单好用。

## ICCV
### 2021
- Incorporating Learnable Membrane Time Constant to Enhance Learning of Spiking Neural Networks. (YuZhaofei) [Link](https://arxiv.org/pdf/2007.05785.pdf)
    > describe: Rate-based SG. 对膜电压时间常数采用基于梯度的方式优化。
