# IP_LAP: Identity-Preserving Talking Face Generation with Landmark and Appearance Priors （CVPR 2023）

****(plan to complete the project before May 15th)****

Pytorch implementation for our CVPR2023 paper "****I****dentity-****P****reserving Talking Face Generation with ****L****andmark and ****A****ppearance ****P****riors".

<img src='./CVPR2023framework.png' width=900>



[[Paper]](https://arxiv.org/abs/coming_soon) [[Demo Video]](https://youtu.be/wtb689iTJC8)

## Requirements
- Python 3.7.13
- Pytorch 1.10.0
- torchvision 0.11.0

We conduct the experiments with 4 24G RTX3090 on CUDA 11.1. For more details, please refer to the `requirements.txt`. We recommand to 
```
pip install -r requirements.txt
```

## Test
download the pretrain models from [[oneDrive]](https://1drv.ms/f/s!Amqu9u09qiUGi7UJIADzCCC9rThkpQ?e=P1jG5N) or [[jianguoyun]](https://www.jianguoyun.com/p/DeXpK34QgZ-EChjI9YcFIAA), and place them to the the `test/checkpoints` 








## Train

### Preprare and Preprocess[LRS2](https://www.robots.ox.ac.uk/~vgg/data/lip_reading/lrs2.html) dataset


### Train Landmark generator
```
CUDA_VISIBLE_DEVICES=0 python train_landmarks_generator.py --pre_audio_root ./lrs2_audio/ --landmarks_root ./lrs2_landmarks/
```

### Train video renderer




## Acknowledgement
This project is built upon the publicly available code [DFRF](https://github.com/sstzal/DFRF) and [Wav2Lip](https://github.com/Rudrabha/Wav2Lip/tree/master). Thanks the authors of DFRF and Wav2Lip for making their excellent work and codes publicly available.




## Citation
Please cite the following paper if you use this repository in your reseach.
```
@inproceedings{zhong2023identity-preserving,
  title={Identity-Preserving Talking Face Generation with Landmark and Appearance Priors},
  author={Weizhi Zhong, Chaowei Fang, Yinqi Cai, Pengxu Wei, Gangming Zhao, Liang Lin, Guanbin Li},
  booktitle="Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition",
  year={2023}
}
```



