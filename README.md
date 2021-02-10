For producing 3D figures in paper "Out-distribution Training Confers Robustness to Deep Neural Networks "

# Summary

We argue and empirically showed that a minimally-modified vanilla CNN, which a vanilla CNN with an extra class added to its output-- call it as Augmented CNN, has the capacity to properly recognize **unseen OOD sets** and some types of adversarial examples, **if it is trained on an appropriate Out-of-Distribution set.** 


In below, the feature space of 3 CNNs for a given in-distribution task (CIFAR-10) are exhibited; I) vanilla CNN; II) A-CNN* (trained a proper OOD set--CIFAR-100), and III) A-CNN (trained on an improper training OOD set--SVHN). In each row, an OOD set or a set of adversarial examples, along with the in-distribution samples, are represented in the feature spaces of these CNN. Note that how the unseen OOD samples (SVHN) and a portion of unseen adversarial examples are disentangled from the in-distribution sub-manifolds in the feature space of A-CNN*.


| OOD set      	|	Vanilla CNN	|	A-CNN* (C100)	|	A-CNN (SVHN)	|
| :------------:| :-------------------:	| :-------------------: |	:----------:	|
|**C100**| <img src='gif_PCA_Chap4/CIFAR10/cnn_c100.gif' width="250" height="250" align="center" />| <img src='gif_PCA_Chap4/CIFAR10/acnn_c100_c100.gif' width="250" height="250" align="center" /> | <img src='gif_PCA_Chap4/CIFAR10/acnn_svhn_c100.gif' width="250" height="250" align="center"/>
|**SVHN**| <img src='gif_PCA_Chap4/CIFAR10/cnn_svhn.gif' width="250" height="250" align="center"/> | <img src='gif_PCA_Chap4/CIFAR10/acnn_c100_svhn.gif' width="250" height="250" align="center"/> |<img src='gif_PCA_Chap4/CIFAR10/acnn_svhn_svhn.gif' width="250" height="250" align="center"/>
|**FGS**| <img src='gif_PCA_Chap4/CIFAR10/cnn_fgs.gif' width="250" height="250" align="center"/> | <img src='gif_PCA_Chap4/CIFAR10/acnn_c100_fgs.gif' width="250" height="250" align="center"/> |<img src='gif_PCA_Chap4/CIFAR10/acnn_svhn_fgs.gif' width="250" height="250" align="center"/>
|**T-FGS**| <img src='gif_PCA_Chap4/CIFAR10/cnn_tfgs.gif' width="250" height="250" align="center"/> | <img src='gif_PCA_Chap4/CIFAR10/acnn_c100_tfgs.gif' width="250" height="250" align="center"/> |<img src='gif_PCA_Chap4/CIFAR10/acnn_svhn_tfgs.gif' width="250" height="250" align="center"/>


## How to recognize an OOD set is proper?
In another paper, We hypothesize that an OOD set is proper if it can cover (protect) in-distribution's sub-manifolds, then propose 3 metrics for recognizing a protective OOD set.

Please visit our another paper, published in ECAI2020, (read here)[http://ecai2020.eu/papers/1553_paper.pdf] or (watch here)[https://screencast-o-matic.com/watch/cYjhc0Gng3]. 

