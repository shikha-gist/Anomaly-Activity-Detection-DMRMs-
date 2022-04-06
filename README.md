# Anomaly-Activity-Detection-DMRMs


## Abstract
Given the scarcity of annotated datasets, learning the context-dependency of anomalous events as well as mitigating false alarms represent challenges in the task of anomalous activity detection. We propose a framework, Deep-network with Multiple Ranking Measures(D.M.R.M.s), which addresses context-dependency using a joint learning technique for motion and appearance features. In D.M.R.M.s, the spatial-time-dependent features are extracted from a video using a 3D residual network(ResNet), and deep motion features are extracted by integrating the motion flow maps' information with the 3D ResNet. Afterward, the extracted features are fused for joint learning. This data fusion is then passed through a deep neural network for deep multiple instance learning(D.M.I.L.)to learn the context-dependency in a weakly-supervised manner using the proposed multiple ranking measures(M.R.M.s). These M.R.M.s consider multiple measures of false alarms, and the network is trained with both normal and anomalous events, thus lowering the false alarm rate. Meanwhile, in the inference phase, the network predicts each frame's abnormality score along with the localization of moving objects using motion flow maps. A higher abnormality score indicates the presence of an anomalous event. Experimental results on two recent and challenging datasets demonstrate that our proposed framework improves the area under the curve(A.U.C.)score by6.5%compared to the state-of-the-art method on the UCF-Crime dataset and shows A.U.C. of68.5%on theShanghaiTech dataset.

![alt text](https://github.com/shikha-gist/Anomaly-Activity-Detection-DMRMs-/blob/main/arch.png)

## DMRMs Frame-level AUC (in %) Evaluation on UCF-Crime and ShanghaiTech Datasets
Model | UCF-Crime | ShanghaiTech  
--- | --- | --- 
DMRMs | 81.9 | 68.5 

[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/anomalous-event-recognition-in-videos-based/anomaly-detection-in-surveillance-videos-on)](https://paperswithcode.com/sota/anomaly-detection-in-surveillance-videos-on?p=anomalous-event-recognition-in-videos-based)
