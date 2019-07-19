
# Localization-Aware Meta Tracker guided with Adversarial Features
This repository includes the code for tracker LMT.

**Localization-Aware Meta Tracker guided with Adversarial Features**   paper line coming soon

### Pytorch Version 

Pytorch implementation is available at [LMT_pytorch](https://github.com/HQUCV/LMT_tracker/).

![](../master/pipeline.jpg)

The overall framework of our LMT tracker. It is composed of three components: (1) Feature extraction network, (2) Classification network, and (3) IoU prediction network.  We use the predicted IoU to adjust the classification scores, and choose the top K candidate patches according to the classification scores. Finally, we use bounding box regression to further fine-tune the location of the object.

### Abstract
Deep learning has recently shown great potentials in learning powerful features for visual tracking. However, most of the deep learning based trackers neglect localization accuracy in the evaluation process of candidates. What's more, they usually over-rely on the discriminative features in a single frame in the training process. Consequently, they may fail when the discriminative features are occluded or changed in the tracking phase. In this work, we propose a novel localization-aware meta tracker guided with adversarial features (named LMT) to address the above issues.  First of all, we design a novel Intersection over Union guided method to effectively balance the problem of classification and localization accuracy. To further improve the robustness of our classifier, we creatively use adversarial features during offline training phase.  Those adversarial features can effectively guide the classifier in learning how to better deal with the situation where the discriminative features are occluded or changed. Finally, benefiting from meta learning, our algorithm only needs to perform one iterative update on the first frame and it can perform well on the tracking sceneries. Extensive experiments demonstrate the outstanding performance of our LMT tracker compared with state-of-the-art trackers on three benchmarks: OTB-2015, VOT-2016, and VOT-2018.

### Result

[result.pdf](../master/result.pdf).

### License
Licensed under an MIT license.

### Citation
If you find this work useful for your research, please consider citing our work:
```
@inproceedings{LMT,
    title={Localization-Aware Meta Tracker Guided with Adversarial Features},
    author={Yiting Lin, Bineng Zhong, Guorong Li, Sicheng Zhao, Ziyi Chen, and Wentao FanWang},
    booktitle={IEEE ACCESS},
    year={2019}
}  
```

### Contact
If you have any questions, please feel free to contact 893448256@qq.com
