# My_Thesis_master_2023
硕士学位论文《基于深度学习脑电解码的智能脑机接口系统研究》，Latex版本。
Master's thesis "Research on Intelligent Brain-Computer Interface System based on Deep Learning EEG Signal Decoding", Latex version.

# 摘要：
脑机接口（BCI），作为人机交互的终极手段，在众多领域具有巨大的发展潜力。基于脑电图（EEG）的BCI系统由于其较低的使用成本和优秀的时间分辨率成为了辨识人脑状态和运动意图的有效手段之一。本课题设计了一套基于EEG的BCI系统——JS-AINS-40。该系统实现了对使用者EEG信号的采集，同时利用基于深度学习的辨识算法准确解码人脑状态与运动意图。

本课题设计的JS-AINS-40系统，通过采集模块实现对40通道EEG数据的同步采样，并经由下位机程序将EEG数据传输至上位机。上位机软件可以对数据进行实时保存、可视化以及类别标注。该系统具备高精度、高共模抑制比以及低噪声等优点，已通过医疗电气设备电磁兼容性检验，性能符合国家标准。

本课题设计的JS-AINS-40系统，针对具体的EEG数据范式分别设计了对应的解码算法。针对被动范式的情绪与疲劳EEG信号，引入结合自适应与早停机制的神经架构搜索（NAS）算法，成功解决当下面向被动范式EEG的深度学习模型设计复杂，调参耗时等问题。搜索得到的网络模型在公开情绪数据集，公开疲劳数据集以及基于JS-AINS-40系统自主采集的情绪数据集上分别得到82.96\%，84.63\%和78.50\%的分类辨识精度，在与其他先进算法的对比中极具竞争力。

针对主动范式中的运动想象EEG信号，引入由特征提取器、动态注意力模块和基于面向域分类器的迭代自训练策略组成的无监督域适应（UDA）框架。成功解决了由于该范式的EEG数据样本数量少，样本间差异大，不同想象动作脑区重叠所带来的模型辨识性能下降问题。使得BCI系统在同时跨被试、跨时段以及多想象类别的实际场景中的应用成为可能。在三个公开的运动想象数据集和基于JS-AINS-40系统自主采集的运动想象数据集上，该辨识算法分别取得了69.51\%、82.38\%，90.98\%以及70.08\%的辨识精度，成功击败了当前的最优模型。

所有的实验结果表明，本课题所设计的JS-AINS-40系统能够满足对于高质量脑电信号采集，人脑状态与意图解码的需求。

# Abstract

Brain computer interface (BCI), the ultimate means of human-computer interaction, has excellent potential for development in many fields. Electroencephalography (EEG)-based BCI system has become one of the effective means for recognizing the states and motor intentions of the human brain, due to their low cost and excellent temporal resolution. The JS-AINS-40, an EEG-based BCI system, is designed to capture the EEG signal and translate the human brain intentions using deep learning-based recognition algorithms.

The JS-AINS-40 system is designed to synchronize the sampling of the 40 channels EEG data via the acquisition module and to transmit the data to the host computer. The data is saved, visualized and labeled in real time by the host computer software. The JS-AINS-40 system has the advantages of high precision, high common-mode rejection ratio and low noise, etc. It has passed the electromagnetic compatibility inspection of medical electrical equipment, and its performance is in line with national standards.

The JS-AINS-40 system designed in this project has corresponding decoding algorithms for different EEG data paradigms. Aiming at the emotion and fatigue EEG signals of the passive paradigm, the neural architecture search (NAS) algorithm combined with adaptive and early stop mechanism is introduced. It successfully solves the problems of complex design and time-consuming parameter adjustment of the current deep learning model. The networks obtained by searching get 82.96\%, 84.63\% and 78.50\% classification accuracy respectively on the public emotion dataset, the public fatigue dataset and the emotion dataset collected based on the JS-AINS-40 system. The final results are very competitive with other advanced algorithms.

An unsupervised domain adaptation (UDA) framework consisting of a feature extractor, a dynamic attention module and a domain-oriented classifier-based iterative self-training, is introduced for motor imagery EEG signals of active paradigm. It successfully solves the problem of model identification performance degradation caused by the small number of EEG samples in this paradigm, the large difference between features, and overlapping brain regions of different imagery movements. This framework makes it possible to apply the BCI system in real scenarios of simultaneous cross-subject, cross-time and multiple motor imagery categories. On three public motor imagery datasets and one dataset collected by JS-AINS 40 system, the proposed algorithm achieves 69.51\%, 82.38\%, 90.98\% and 70.08\% identification accuracy, which successfully beats the current optimal model.

All the experimental results show that the JS-AINS-40 system designed in this project can meet the requirements for high-quality EEG signal acquisition and decoding of the states or intentions of the human brain.

# Acknowledgements

- [tjuthesis](https://code.google.com/archive/p/tjuthesis/)
- [TJUThesisLatexTemplate](https://github.com/twtstudio/TJUThesisLatexTemplate)
- [tjuthesis_master_2016](https://github.com/jiangqideng/tjuthesis_master_2016)



