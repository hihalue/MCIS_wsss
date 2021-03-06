## MCIS_wsss

Code for Mining Cross-Image Semantics for Weakly Supervised Semantic Segmentation [ECCV 2020 (oral)]

CVPR 2020 [Learning from Imperfect Data (LID)](https://lidchallenge.github.io) workshop Best Paper Award and winner solution in WSSS Track of CVPR2020 LID challenge

===========================================================================

Authors: [Guolei Sun](https://github.com/GuoleiSun), [Wenguan Wang](https://sites.google.com/view/wenguanwang), [Jifeng Dai](https://jifengdai.org/), Luc Van Gool.

===========================================================================

![block images](https://github.com/GuoleiSun/MCIS_wsss/blob/master/framework.png)

### Quick Start

#### Test

1. Install Caffe: install [prerequisites](https://caffe.berkeleyvision.org/install_apt.html), then go to segmentation folder and run "make all -j4 && make pycaffe" to compile. To continue, make sure Caffe is installed correctly by referring to [Caffe](https://caffe.berkeleyvision.org/installation.html#compilation).

2. Download the [PASCAL VOC 2012](https://drive.google.com/open?id=1uh5bWXvLOpE-WZUUtO77uwCB4Qnh6d7X) and pretrained segmentation [model](https://drive.google.com/file/d/1BgT8nTIs4ts_W_7JX0WTg5jb5EetnAVz/view?usp=sharing). Put the segmentation model in folder segmentation/examples/seg/exp2/model/

3. Go to segmentation/examples/seg, change the dataset path when necessary, and run "python eval_res.py gpu_id exp2 model". You will get mIoU score of 66.2 on PASCAL VOC12 val set.

#### To do

coattention classifer

### Citation
If you find the code and dataset useful in your research, please consider citing:

@InProceedings{sun2020mining,

  title={Mining Cross-Image Semantics for Weakly Supervised Semantic Segmentation},
  
  author={Sun, Guolei and Wang, Wenguan and Dai, Jifeng and Van Gool, Luc},
  
  booktitle={ECCV},
  
  year={2020}
}

### Acknowledgements 

This repository is based on [OAA](https://github.com/PengtaoJiang/OAA), thanks for their excellent work.

For questions, please contact sunguolei.kaust@gmail.com
