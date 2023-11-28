# Global-Local Path Networks for Monocular Depth Estimation with Vertical CutDepth [[Paper]](https://arxiv.org/abs/2201.07436)

[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/global-local-path-networks-for-monocular/monocular-depth-estimation-on-nyu-depth-v2)](https://paperswithcode.com/sota/monocular-depth-estimation-on-nyu-depth-v2?p=global-local-path-networks-for-monocular)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/global-local-path-networks-for-monocular/monocular-depth-estimation-on-kitti-eigen)](https://paperswithcode.com/sota/monocular-depth-estimation-on-kitti-eigen?p=global-local-path-networks-for-monocular)

### Downloads
- [[Downloads]](https://drive.google.com/drive/folders/17yYbLZS2uQ6UVn5ET9RhVL0y_X3Ipl5_?usp=sharing) Trained ckpt files for NYU Depth V2 and KITTI

### Requirements
Tested on 
```
python==3.8.3
torch==1.11.0+cu113
h5py==3.10.0
scipy==1.10.1
opencv-python==4.8.1.78
mmcv==1.4.3
timm==0.9.12
albumentations==1.3.1
tensorboardX==2.6.2.2
gdown==4.7.1
```

```
$ pip install -r requirements.txt
```
### Inference and Evaluate

#### Dataset

###### KITTI
Download annotated depth maps data set (14GB) from [[link]](http://www.cvlibs.net/datasets/kitti/eval_depth.php?benchmark=depth_prediction) into ./datasets/kitti/data_depth_annotated
```
$ cd datasets/kitti/data_depth_annotated/
$ unzip data_depth_annotated.zip
```



#### Inference

- Inference with image directory
  ```
  $ python test.py --dataset imagepath --data_path <dir_to_imgs> --save_visualize
  ```
  
### License
For non-commercial purpose only (research, evaluation etc). We will update the license soon.

### Citation

```
@article{kim2022global,
  title={Global-Local Path Networks for Monocular Depth Estimation with Vertical CutDepth},
  author={Kim, Doyeon and Ga, Woonghyun and Ahn, Pyungwhan and Joo, Donggyu and Chun, Sehwan and Kim, Junmo},
  journal={arXiv preprint arXiv:2201.07436},
  year={2022}
}
```

### References

[1] From Big to Small: Multi-Scale Local Planar Guidance for Monocular Depth Estimation. [[code]](https://github.com/cleinc/bts)

[2] SegFormer: Simple and Efficient Design for Semantic Segmentation with Transformers. [[code]](https://github.com/NVlabs/SegFormer)
