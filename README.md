## Graduation thesis
毕业论文 上下文特征引导的显著性目标检测方法研究

## Proposed Method

<div align="center">
  <img src="https://github.com/1291869157/BENet/blob/main/fig11.png" width="80%">
</div>

In this paper, we propose a novel boundary enhance network. The model contains multiple sub-networks. The Progressive Feature Extraction Module (PFEM) is used to capture the boundary features and salient object features of salient objects at multiple scales. The Edge Enhance Module (EEM) consists of a series of Adaptive Edge Fusion Modules (AEFM) to balance the fusion of edge features and salient object features. To make the network pay more attention to the details of the boundary region, we design a edge enhancement loss to give higher weights near the boundary. 

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



