---
layout: default
---

## Introduction
MVIdeoGallery is an open-sourced video understanding toolbox based on [PyTorch](https://pytorch.org/) covering multi-object tracking and action detection.
In MVIdeoGallery, we released the first one-stage multi-object tracking (MOT) system **TubeTK** that can achieve 66.9 MOTA on [MOT-16](https://motchallenge.net/results/MOT16) dataset and 63 MOTA on [MOT-17](https://motchallenge.net/results/MOT17) dataset.
For action detection, we released an efficient model **AlphAction**, which is the first open-source project that achieves 30+ mAP (32.4 mAP) with single model on [AVA](https://research.google.com/ava/) dataset.

## Quick Start
### pip
Run this command:
```shell
pip install mvideogallery
```

### from source
Clone repository from github:
```bash
git clone https://github.com/ mvideogallery
cd mvideogallery
```

Setup and install MVIdeoGallery:
```bash
python setup.py build install
```

## Features & Capabilities 
* #### Multi-Object Tracking
<img src="https://github.com/liyz15/3DTracking/raw/clean_version/assets/demo.gif" width = "600" align=center />
  * Accurate end-to-end multi-object tracking.
  * Do not need any ready-made image-level object deteaction models.
  * Pre-trained model for pedestrian tracking. 
  * Input: Frame list; video.
  * Output: Videos decorated by colored bounding-box; Btube lists.
  * For details usages, see our [docs]().
* #### Action recognition

## Paper and Citations
```
@inproceedings{pang2020tubeTK,
  title={TubeTK: Adopting Tubes to Track Multi-Object in a One-Step Training Model},
  author={Bo, Pang and Yizhuo, Li and Yifan, Zhang and Muchen, Li and Lu, Cewu},
  booktitle={CVPR},
  year={2020}
}

@article{tang2020asynchronous,
  title={Asynchronous Interaction Aggregation for Action Detection},
  author={Tang, Jiajun and Xia, Jin and Mu, Xinzhi and Pang, Bo and Lu, Cewu},
  journal={arXiv preprint arXiv:2004.07485},
  year={2020}
}
```

## Maintainers
This project is open-sourced and maintained by Machine Vision and Intelligence Group ([MVIG](http://mvig.sjtu.edu.cn)) in Shanghai Jiao Tong University.

