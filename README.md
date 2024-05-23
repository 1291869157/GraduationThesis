## Graduation thesis
毕业论文 上下文特征引导的显著性目标检测方法研究

## 摘要
   目前，基于单张图像的显著性目标检测受制于上下文信息和空间信息的缺失，对图像的质量要求较高。当图像的拍摄角度变化或是光照导致对比度较低时，会对最终的检测结果造成比较大的影响。同时，由于当前的显著性目标检测方法严重依赖于准确的像素级注释,为了减少注释工作量，一些基于弱监督的显著性目标检测方法也被提出，并且其中上下文推理的难度更高。如何更好地利用上下文信息弥补稀疏的弱标签也成为了亟待解决的问题。因此，本课题旨在利用图像中潜在的多种上下文特征引导网络更好地区分显著目标与背景的边界，提高现有全监督以及弱监督显著性目标检测方法的准确率，本文的主要贡献如下：<br>
   第一，针对全监督方法中上下文信息表示不足，无法得到显著性目标精确的轮廓和边界的问题，本文提出了一种用于显著性目标检测的边界自适应增强网络，显式地引入了边缘信息，并通过神经网络自适应地为边界特征和显著对象特征分配权重和提出边界增强损失，使网络更多地关注到边界区域潜在的兴趣点，极大提升了预测结果的边界质量。<br>
   第二，针对弱监督显著性目标检测中训练数据标注稀疏的问题，本文进一步对训练过程中的上下文信息进行了增强和关联，探讨了上下文信息之间的长距离依赖性对能量传播和模型性能的影响，通过构建图表示来全局推断显著性区域之间的关系。具体来说，本文引入了双流交互式图推理管道来对高级表示进行建模，并结合图合作单元来自适应地从表示中选择和互补上下文信息。此外，文中显式地引入了边界上下文信息弥补涂鸦数据中缺乏的结构信息。最后，提出了一种密集融合策略，以多指导方式聚合多源上下文信息，从而获得完整的全局信息。
   第三，针对弱监督显著性目标检测中存在的非显著性抑制问题，本文从序列角度重新思考了显著性目标检测问题，使用图像块来充当上下文信息的载体。具体来说，本文提出了一种多尺度图像块推理网络，利用视觉transformer的高质量表征有效提取了显著对象的全局上下文特征。此外，文中改进了传统图像块的推理结构，以令牌形式交互边缘和显著性信息，极大地改善了非显著性抑制问题。


## Experiment
#### Visual Comparison
<div align="center">
  <img src="https://github.com/1291869157/BENet/blob/main/fig12.png" width="80%">
</div>
Since the methods of comparison lack sufficient boundary information, other's prediction boundaries are blurred. While our method balances and strengthens the boundary information, which can better identify interest points near the boundary.

#### Quantitative Comparison
<div align="center">
  <img src="https://github.com/1291869157/BENet/blob/main/fig13.jpg" width="60%">
</div>
We qualitatively compare the methods from the two metrics. As shown in table, we can see that our BENet model achieves the best metrics on most datasets, which shows that our model is effective and robust.



