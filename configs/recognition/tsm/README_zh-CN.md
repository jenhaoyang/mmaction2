# TSM

## 简介

<!-- [ALGORITHM] -->

```BibTeX
@inproceedings{lin2019tsm,
  title={TSM: Temporal Shift Module for Efficient Video Understanding},
  author={Lin, Ji and Gan, Chuang and Han, Song},
  booktitle={Proceedings of the IEEE International Conference on Computer Vision},
  year={2019}
}
```

<!-- [BACKBONE] -->

```BibTeX
@article{NonLocal2018,
  author =   {Xiaolong Wang and Ross Girshick and Abhinav Gupta and Kaiming He},
  title =    {Non-local Neural Networks},
  journal =  {CVPR},
  year =     {2018}
}
```

## 模型库

### Kinetics-400

|配置文件 | 分辨率 | GPU 数量 | 主干网络 | 预训练 | top1 准确率 | top5 准确率 | 参考代码的 top1 准确率 | 参考代码的 top5 准确率 | 推理时间 (video/s) | GPU 显存占用 (M)| ckpt | log| json|
|:--|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|
|[tsm_r50_1x1x8_50e_kinetics400_rgb](/configs/recognition/tsm/tsm_r50_1x1x8_50e_kinetics400_rgb.py) |340x256|8| ResNet50| ImageNet |70.24|89.56|[70.36](https://github.com/mit-han-lab/temporal-shift-module/blob/8d53d6fda40bea2f1b37a6095279c4b454d672bd/scripts/train_tsm_kinetics_rgb_8f.sh)|[89.49](https://github.com/mit-han-lab/temporal-shift-module/blob/8d53d6fda40bea2f1b37a6095279c4b454d672bd/scripts/train_tsm_kinetics_rgb_8f.sh)|74.0 (8x1 frames)| 7079 | [ckpt](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_1x1x8_50e_kinetics400_rgb/tsm_r50_1x1x8_50e_kinetics400_rgb_20200607-af7fb746.pth) | [log](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_1x1x8_50e_kinetics400_rgb/20200607_211800.log)| [json](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_1x1x8_50e_kinetics400_rgb/20200607_211800.log.json)|
|[tsm_r50_1x1x8_50e_kinetics400_rgb](/configs/recognition/tsm/tsm_r50_1x1x8_50e_kinetics400_rgb.py) |短边 256|8| ResNet50| ImageNet |70.59|89.52|x|x|x|7079|[ckpt](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_256p_1x1x8_50e_kinetics400_rgb/tsm_r50_256p_1x1x8_50e_kinetics400_rgb_20200726-020785e2.pth)|[log](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_256p_1x1x8_50e_kinetics400_rgb/20200725_031623.log)|[json](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_256p_1x1x8_50e_kinetics400_rgb/20200725_031623.log.json)|
|[tsm_r50_1x1x8_50e_kinetics400_rgb](/configs/recognition/tsm/tsm_r50_1x1x8_50e_kinetics400_rgb.py) |短边 320|8| ResNet50| ImageNet |70.73|89.81|x|x|x|7079|[ckpt](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_1x1x8_50e_kinetics400_rgb/tsm_r50_1x1x8_50e_kinetics400_rgb_20210701-68d582b4.pth)|[log](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_1x1x8_50e_kinetics400_rgb/20210616_021451.log)|[json](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_1x1x8_50e_kinetics400_rgb/20210616_021451.log.json)|
|[tsm_r50_1x1x8_100e_kinetics400_rgb](/configs/recognition/tsm/tsm_r50_1x1x8_100e_kinetics400_rgb.py) |短边 320|8| ResNet50| ImageNet |71.90|90.03|x|x|x|7079|[ckpt](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_1x1x8_100e_kinetics400_rgb/tsm_r50_1x1x8_100e_kinetics400_rgb_20210701-7ff22268.pth)|[log](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_1x1x8_100e_kinetics400_rgb/20210617_103543.log)|[json](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_1x1x8_100e_kinetics400_rgb/20210617_103543.log.json)|
|[tsm_r50_gpu_normalize_1x1x8_50e_kinetics400_rgb.py](/configs/recognition/tsm/tsm_r50_gpu_normalize_1x1x8_50e_kinetics400_rgb.py) |短边 256|8| ResNet50| ImageNet |70.48|89.40|x|x|x|7076|[ckpt](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_gpu_normalize_1x1x8_50e_kinetics400_rgb/tsm_r50_gpu_normalize_1x1x8_50e_kinetics400_rgb_20210219-bf96e6cc.pth)|[log](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_gpu_normalize_1x1x8_50e_kinetics400_rgb/tsm_r50_gpu_normalize_1x1x8_50e_kinetics400_rgb_20210219.log)|[json](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_gpu_normalize_1x1x8_50e_kinetics400_rgb/tsm_r50_gpu_normalize_1x1x8_50e_kinetics400_rgb_20210219.json)|
|[tsm_r50_video_1x1x8_50e_kinetics400_rgb](/configs/recognition/tsm/tsm_r50_video_1x1x8_50e_kinetics400_rgb.py) |短边 256|8| ResNet50| ImageNet |70.25|89.66|[70.36](https://github.com/mit-han-lab/temporal-shift-module/blob/8d53d6fda40bea2f1b37a6095279c4b454d672bd/scripts/train_tsm_kinetics_rgb_8f.sh)|[89.49](https://github.com/mit-han-lab/temporal-shift-module/blob/8d53d6fda40bea2f1b37a6095279c4b454d672bd/scripts/train_tsm_kinetics_rgb_8f.sh)|74.0 (8x1 frames)| 7077 | [ckpt]( https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_video_1x1x8_100e_kinetics400_rgb/tsm_r50_video_1x1x8_100e_kinetics400_rgb_20200702-a77f4328.pth) | [log](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_video_1x1x8_100e_kinetics400_rgb/tsm_r50_video_2d_1x1x8_50e_kinetics400_rgb.log)| [json](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_video_1x1x8_100e_kinetics400_rgb/tsm_r50_video_2d_1x1x8_50e_kinetics400_rgb.log.json)|
|[tsm_r50_dense_1x1x8_50e_kinetics400_rgb](/configs/recognition/tsm/tsm_r50_dense_1x1x8_50e_kinetics400_rgb.py) |短边 320|8| ResNet50 | ImageNet|73.46|90.84|x|x|x|7079|[ckpt](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_dense_1x1x8_50e_kinetics400_rgb/tsm_r50_dense_1x1x8_50e_kinetics400_rgb_20210701-a54ff3d3.pth)|[log](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_dense_1x1x8_50e_kinetics400_rgb/20210617_103245.log)|[json](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_dense_1x1x8_50e_kinetics400_rgb/20210617_103245.log.json)|
|[tsm_r50_dense_1x1x8_100e_kinetics400_rgb](/configs/recognition/tsm/tsm_r50_dense_1x1x8_100e_kinetics400_rgb.py) |短边 320|8| ResNet50 | ImageNet|74.55|91.74|x|x|x|7079|[ckpt](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_dense_1x1x8_100e_kinetics400_rgb/tsm_r50_dense_1x1x8_100e_kinetics400_rgb_20210701-e3e5e97f.pth)|[log](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_dense_1x1x8_100e_kinetics400_rgb/20210613_034931.log)|[json](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_dense_1x1x8_100e_kinetics400_rgb/20210613_034931.log.json)|
|[tsm_r50_1x1x16_50e_kinetics400_rgb](/configs/recognition/tsm/tsm_r50_1x1x16_50e_kinetics400_rgb.py) |340x256|8| ResNet50| ImageNet |72.09|90.37|[70.67](https://github.com/mit-han-lab/temporal-shift-module/blob/8d53d6fda40bea2f1b37a6095279c4b454d672bd/scripts/train_tsm_kinetics_rgb_16f.sh)|[89.98](https://github.com/mit-han-lab/temporal-shift-module/blob/8d53d6fda40bea2f1b37a6095279c4b454d672bd/scripts/train_tsm_kinetics_rgb_16f.sh)|47.0 (16x1 frames)| 10404  | [ckpt](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_1x1x16_50e_kinetics400_rgb/tsm_r50_340x256_1x1x16_50e_kinetics400_rgb_20201011-2f27f229.pth) | [log](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_1x1x16_50e_kinetics400_rgb/20201011_205356.log)| [json](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_1x1x16_50e_kinetics400_rgb/20201011_205356.log.json)|
|[tsm_r50_1x1x16_50e_kinetics400_rgb](/configs/recognition/tsm/tsm_r50_1x1x16_50e_kinetics400_rgb.py) |短边 256|8x4| ResNet50| ImageNet |71.89|90.73|x|x|x|10398|[ckpt](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_256p_1x1x16_50e_kinetics400_rgb/tsm_r50_256p_1x1x16_50e_kinetics400_rgb_20201010-85645c2a.pth)|[log](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_256p_1x1x16_50e_kinetics400_rgb/20201010_224825.log)|[json](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_256p_1x1x16_50e_kinetics400_rgb/20201010_224825.log.json)|
|[tsm_r50_1x1x16_100e_kinetics400_rgb](/configs/recognition/tsm/tsm_r50_1x1x16_100e_kinetics400_rgb.py) |短边 320|8| ResNet50| ImageNet |72.80|90.75|x|x|x|10398|[ckpt](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_1x1x16_100e_kinetics400_rgb/tsm_r50_1x1x16_100e_kinetics400_rgb_20210701-41ac92b9.pth)|[log](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_1x1x16_100e_kinetics400_rgb/20210618_193859.log)|[json](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_1x1x16_100e_kinetics400_rgb/20210618_193859.log.json)|
|[tsm_nl_embedded_gaussian_r50_1x1x8_50e_kinetics400_rgb](/configs/recognition/tsm/tsm_nl_embedded_gaussian_r50_1x1x8_50e_kinetics400_rgb.py)|短边 320|8x4| ResNet50| ImageNet |72.03|90.25|71.81|90.36|x|8931|[ckpt](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_nl_embedded_gaussian_r50_1x1x8_50e_kinetics400_rgb/tsm_nl_embedded_gaussian_r50_1x1x8_50e_kinetics400_rgb_20200724-f00f1336.pth)|[log](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_nl_embedded_gaussian_r50_1x1x8_50e_kinetics400_rgb/20200724_120023.log)|[json](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_nl_embedded_gaussian_r50_1x1x8_50e_kinetics400_rgb/20200724_120023.log.json)|
|[tsm_nl_gaussian_r50_1x1x8_50e_kinetics400_rgb](/configs/recognition/tsm/tsm_nl_gaussian_r50_1x1x8_50e_kinetics400_rgb.py)|短边 320|8x4| ResNet50| ImageNet |70.70|89.90|x|x|x|10125|[ckpt](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_nl_gaussian_r50_1x1x8_50e_kinetics400_rgb/tsm_nl_gaussian_r50_1x1x8_50e_kinetics400_rgb_20200816-b93fd297.pth)|[log](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_nl_gaussian_r50_1x1x8_50e_kinetics400_rgb/20200815_210253.log)|[json](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_nl_gaussian_r50_1x1x8_50e_kinetics400_rgb/20200815_210253.log.json)|
|[tsm_nl_dot_product_r50_1x1x8_50e_kinetics400_rgb](/configs/recognition/tsm/tsm_nl_dot_product_r50_1x1x8_50e_kinetics400_rgb.py)|短边 320|8x4|ResNet50| ImageNet |71.60|90.34|x|x|x|8358|[ckpt](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_nl_dot_product_r50_1x1x8_50e_kinetics400_rgb/tsm_nl_dot_product_r50_1x1x8_50e_kinetics400_rgb_20200724-d8ad84d2.pth)|[log](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_nl_dot_product_r50_1x1x8_50e_kinetics400_rgb/20200723_220442.log)|[json](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_nl_dot_product_r50_1x1x8_50e_kinetics400_rgb/20200723_220442.log.json)|
|[tsm_mobilenetv2_dense_1x1x8_100e_kinetics400_rgb](/configs/recognition/tsm/tsm_mobilenetv2_dense_1x1x8_100e_kinetics400_rgb.py)|短边 320|8|MobileNetV2| ImageNet |68.46|88.64|x|x|x|3385|[ckpt](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_mobilenetv2_dense_1x1x8_100e_kinetics400_rgb/tsm_mobilenetv2_dense_320p_1x1x8_100e_kinetics400_rgb_20210202-61135809.pth)|[log](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_mobilenetv2_dense_1x1x8_100e_kinetics400_rgb/20210129_024936.log)|[json](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_mobilenetv2_dense_1x1x8_100e_kinetics400_rgb/20210129_024936.log.json)|
|[tsm_mobilenetv2_dense_1x1x8_kinetics400_rgb_port](/configs/recognition/tsm/tsm_mobilenetv2_dense_1x1x8_100e_kinetics400_rgb.py)|短边 320|8|MobileNetV2| ImageNet |69.89|89.01|x|x|x|3385|[infer_ckpt](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_mobilenetv2_dense_1x1x8_kinetics400_rgb_port_20210922-aa5cadf6.pth)|x|x|

### Diving48

|配置文件 | GPU 数量 | 主干网络 | 预训练 | top1 准确率| top5 准确率 | GPU 显存占用 (M) | ckpt | log| json|
|:--|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|
|[tsm_r50_video_1x1x8_50e_diving48_rgb](/configs/recognition/tsm/tsm_r50_video_1x1x8_50e_diving48_rgb.py)| 8 | ResNet50 | ImageNet | 75.99 | 97.16 | 7070 | [ckpt](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_video_1x1x8_50e_diving48_rgb/tsm_r50_video_1x1x8_50e_diving48_rgb_20210426-aba5aa3d.pth) | [log](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_video_1x1x8_50e_diving48_rgb/20210426_012424.log) | [json](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_video_1x1x8_50e_diving48_rgb/20210426_012424.log.json)|
|[tsm_r50_video_1x1x16_50e_diving48_rgb](/configs/recognition/tsm/tsm_r50_video_1x1x16_50e_diving48_rgb.py)| 8 | ResNet50 | ImageNet | 81.62 | 97.66 | 7070 | [ckpt](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_video_1x1x16_50e_diving48_rgb/tsm_r50_video_1x1x16_50e_diving48_rgb_20210426-aa9631c0.pth) | [log](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_video_1x1x16_50e_diving48_rgb/20210426_012823.log) | [json](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_video_1x1x16_50e_diving48_rgb/20210426_012823.log.json)|

### Something-Something V1

|配置文件 | 分辨率 | GPU 数量 | 主干网络| 预训练 | top1 准确率 (efficient/accurate)| top5 准确率 (efficient/accurate)| 参考代码的 top1 准确率 (efficient/accurate)| 参考代码的 top5 准确率 (efficient/accurate)| GPU 显存占用 (M)| ckpt | log| json|
|:--|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|
|[tsm_r50_1x1x8_50e_sthv1_rgb](/configs/recognition/tsm/tsm_r50_1x1x8_50e_sthv1_rgb.py) |高 100|8| ResNet50 | ImageNet| 45.58 / 47.70|75.02 / 76.12|[45.50 / 47.33](https://github.com/mit-han-lab/temporal-shift-module/tree/8d53d6fda40bea2f1b37a6095279c4b454d672bd#training)|[74.34 / 76.60](https://github.com/mit-han-lab/temporal-shift-module/tree/8d53d6fda40bea2f1b37a6095279c4b454d672bd#training)| 7077| [ckpt](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_1x1x8_50e_sthv1_rgb/tsm_r50_1x1x8_50e_sthv1_rgb_20210203-01dce462.pth) | [log](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_1x1x8_50e_sthv1_rgb/20210203_150227.log)| [json](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_1x1x8_50e_sthv1_rgb/20210203_150227.log.json)|
|[tsm_r50_flip_1x1x8_50e_sthv1_rgb](/configs/recognition/tsm/tsm_r50_flip_1x1x8_50e_sthv1_rgb.py) |高 100|8| ResNet50 | ImageNet| 47.10 / 48.51|76.02 / 77.56|[45.50 / 47.33](https://github.com/mit-han-lab/temporal-shift-module/tree/8d53d6fda40bea2f1b37a6095279c4b454d672bd#training)|[74.34 / 76.60](https://github.com/mit-han-lab/temporal-shift-module/tree/8d53d6fda40bea2f1b37a6095279c4b454d672bd#training)| 7077| [ckpt](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_flip_1x1x8_50e_sthv1_rgb/tsm_r50_flip_1x1x8_50e_sthv1_rgb_20210203-12596f16.pth) | [log](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_flip_1x1x8_50e_sthv1_rgb/20210203_145829.log)| [json](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_flip_1x1x8_50e_sthv1_rgb/20210203_145829.log.json)|
|[tsm_r50_randaugment_1x1x8_50e_sthv1_rgb](/configs/recognition/tsm/tsm_r50_randaugment_1x1x8_50e_sthv1_rgb.py)| 高 100 |    8     | ResNet50 | ImageNet |          47.16 / 48.90           |          76.07 / 77.92           | [45.50 / 47.33](https://github.com/mit-han-lab/temporal-shift-module/tree/8d53d6fda40bea2f1b37a6095279c4b454d672bd#training) | [74.34 / 76.60](https://github.com/mit-han-lab/temporal-shift-module/tree/8d53d6fda40bea2f1b37a6095279c4b454d672bd#training) |       7077       | [ckpt](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_randaugment_1x1x8_50e_sthv1_rgb/tsm_r50_randaugment_1x1x8_50e_sthv1_rgb_20210324-481268d9.pth) | [log](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_randaugment_1x1x8_50e_sthv1_rgb/tsm_r50_randaugment_1x1x8_50e_sthv1_rgb.log) | [json](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_randaugment_1x1x8_50e_sthv1_rgb/tsm_r50_randaugment_1x1x8_50e_sthv1_rgb.json) |
| [tsm_r50_ptv_randaugment_1x1x8_50e_sthv1_rgb](/configs/recognition/tsm/tsm_r50_ptv_randaugment_1x1x8_50e_sthv1_rgb.py) | 高 100 |    8     | ResNet50 | ImageNet |          47.65 / 48.66           |          76.67 / 77.41           | [45.50 / 47.33](https://github.com/mit-han-lab/temporal-shift-module/tree/8d53d6fda40bea2f1b37a6095279c4b454d672bd#training) | [74.34 / 76.60](https://github.com/mit-han-lab/temporal-shift-module/tree/8d53d6fda40bea2f1b37a6095279c4b454d672bd#training) |       7077       | [ckpt](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_ptv_randaugment_1x1x8_50e_sthv1_rgb/tsm_r50_ptv_randaugment_1x1x8_50e_sthv1_rgb-ee93e5e3.pth) | [log](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_ptv_randaugment_1x1x8_50e_sthv1_rgb/tsm_r50_ptv_randaugment_1x1x8_50e_sthv1_rgb.log) | [json](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_ptv_randaugment_1x1x8_50e_sthv1_rgb/tsm_r50_ptv_randaugment_1x1x8_50e_sthv1_rgb.json) |
| [tsm_r50_ptv_augmix_1x1x8_50e_sthv1_rgb](/configs/recognition/tsm/tsm_r50_ptv_augmix_1x1x8_50e_sthv1_rgb.py) | 高 100 |    8     | ResNet50 | ImageNet |          46.26 / 47.68           |          75.92 / 76.49           | [45.50 / 47.33](https://github.com/mit-han-lab/temporal-shift-module/tree/8d53d6fda40bea2f1b37a6095279c4b454d672bd#training) | [74.34 / 76.60](https://github.com/mit-han-lab/temporal-shift-module/tree/8d53d6fda40bea2f1b37a6095279c4b454d672bd#training) |       7077       | [ckpt](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_ptv_augmix_1x1x8_50e_sthv1_rgb/tsm_r50_ptv_augmix_1x1x8_50e_sthv1_rgb-4f4f4740.pth) | [log](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_ptv_augmix_1x1x8_50e_sthv1_rgb/tsm_r50_ptv_augmix_1x1x8_50e_sthv1_rgb.log) | [json](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_ptv_augmix_1x1x8_50e_sthv1_rgb/tsm_r50_ptv_augmix_1x1x8_50e_sthv1_rgb.json) |
| [tsm_r50_flip_randaugment_1x1x8_50e_sthv1_rgb](/configs/recognition/tsm/tsm_r50_flip_randaugment_1x1x8_50e_sthv1_rgb.py) | 高 100 |    8     | ResNet50 | ImageNet |          47.85 / 50.31           |          76.78 / 78.18           | [45.50 / 47.33](https://github.com/mit-han-lab/temporal-shift-module/tree/8d53d6fda40bea2f1b37a6095279c4b454d672bd#training) | [74.34 / 76.60](https://github.com/mit-han-lab/temporal-shift-module/tree/8d53d6fda40bea2f1b37a6095279c4b454d672bd#training) |7077|[ckpt](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_flip_randaugment_1x1x8_50e_sthv1_rgb/tsm_r50_flip_randaugment_1x1x8_50e_sthv1_rgb_20210324-76937692.pth)|[log](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_flip_randaugment_1x1x8_50e_sthv1_rgb/tsm_r50_flip_randaugment_1x1x8_50e_sthv1_rgb.log)|[json](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_flip_randaugment_1x1x8_50e_sthv1_rgb/tsm_r50_flip_randaugment_1x1x8_50e_sthv1_rgb.json)|
|[tsm_r50_1x1x16_50e_sthv1_rgb](/configs/recognition/tsm/tsm_r50_1x1x16_50e_sthv1_rgb.py)|高 100|8| ResNet50 | ImageNet|47.77 / 49.03|76.82 / 77.83|[47.05 / 48.61](https://github.com/mit-han-lab/temporal-shift-module/tree/8d53d6fda40bea2f1b37a6095279c4b454d672bd#training)|[76.40 / 77.96](https://github.com/mit-han-lab/temporal-shift-module/tree/8d53d6fda40bea2f1b37a6095279c4b454d672bd#training)|10390|[ckpt](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_1x1x16_50e_sthv1_rgb/tsm_r50_1x1x16_50e_sthv1_rgb_20211202-b922e5d2.pth)|[log](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_1x1x16_50e_sthv1_rgb/tsm_r50_1x1x16_50e_sthv1_rgb.log)|[json](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_1x1x16_50e_sthv1_rgb/tsm_r50_1x1x16_50e_sthv1_rgb.json)|
|[tsm_r101_1x1x8_50e_sthv1_rgb](/configs/recognition/tsm/tsm_r101_1x1x8_50e_sthv1_rgb.py)|高 100|8| ResNet50 | ImageNet|46.09 / 48.59|75.41 / 77.10|[46.64 / 48.13](https://github.com/mit-han-lab/temporal-shift-module/tree/8d53d6fda40bea2f1b37a6095279c4b454d672bd#training)|[75.40 / 77.31](https://github.com/mit-han-lab/temporal-shift-module/tree/8d53d6fda40bea2f1b37a6095279c4b454d672bd#training)|9800|[ckpt](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r101_1x1x8_50e_sthv1_rgb/tsm_r101_1x1x8_50e_sthv1_rgb_20201010-43fedf2e.pth)|[log](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r101_1x1x8_50e_sthv1_rgb/tsm_r101_1x1x8_50e_sthv1_rgb.log)|[json](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r101_1x1x8_50e_sthv1_rgb/tsm_r101_1x1x8_50e_sthv1_rgb.json)|

### Something-Something V2

|配置文件 | 分辨率 | GPU 数量 | 主干网络| 预训练 | top1 准确率 (efficient/accurate)| top5 准确率 (efficient/accurate)| 参考代码的 top1 准确率 (efficient/accurate)| 参考代码的 top5 准确率 (efficient/accurate)| GPU 显存占用 (M)| ckpt | log| json|
|:--|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|
|[tsm_r50_1x1x8_50e_sthv2_rgb](/configs/recognition/tsm/tsm_r50_1x1x8_50e_sthv2_rgb.py) |高 256|8| ResNet50| ImageNet |59.11 / 61.82|85.39 / 86.80|[xx / 61.2](https://github.com/mit-han-lab/temporal-shift-module/tree/8d53d6fda40bea2f1b37a6095279c4b454d672bd#training)|[xx / xx](https://github.com/mit-han-lab/temporal-shift-module/tree/8d53d6fda40bea2f1b37a6095279c4b454d672bd#training)| 7069 | [ckpt](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_1x1x8_50e_sthv2_rgb/tsm_r50_256h_1x1x8_50e_sthv2_rgb_20210816-032aa4da.pth) | [log](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_1x1x8_50e_sthv2_rgb/20210816_224310.log) | [json](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_1x1x8_50e_sthv2_rgb/20210816_224310.log.json)|
|[tsm_r50_1x1x16_50e_sthv2_rgb](/configs/recognition/tsm/tsm_r50_1x1x8_50e_sthv2_rgb.py) |高 256|8| ResNet50| ImageNet |61.06 / 63.19|86.66 / 87.93|[xx / 63.1](https://github.com/mit-han-lab/temporal-shift-module/tree/8d53d6fda40bea2f1b37a6095279c4b454d672bd#training)|[xx / xx](https://github.com/mit-han-lab/temporal-shift-module/tree/8d53d6fda40bea2f1b37a6095279c4b454d672bd#training)| 10400 | [ckpt](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_1x1x16_50e_sthv2_rgb/tsm_r50_256h_1x1x16_50e_sthv2_rgb_20210331-0a45549c.pth) | [log](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_1x1x16_50e_sthv2_rgb/20210331_134458.log) | [json](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_1x1x16_50e_sthv2_rgb/20210331_134458.log.json)|
|[tsm_r101_1x1x8_50e_sthv2_rgb](/configs/recognition/tsm/tsm_r101_1x1x8_50e_sthv2_rgb.py) |高 256|8| ResNet101 | ImageNet|60.88 / 63.84|86.56 / 88.30|[xx / 63.3](https://github.com/mit-han-lab/temporal-shift-module/tree/8d53d6fda40bea2f1b37a6095279c4b454d672bd#training)|[xx / xx](https://github.com/mit-han-lab/temporal-shift-module/tree/8d53d6fda40bea2f1b37a6095279c4b454d672bd#training)| 9727 | [ckpt](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r101_1x1x8_50e_sthv2_rgb/tsm_r101_256h_1x1x8_50e_sthv2_rgb_20210401-df97f3e1.pth) | [log](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r101_1x1x8_50e_sthv2_rgb/20210401_143656.log) | [json](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r101_1x1x8_50e_sthv2_rgb/20210401_143656.log.json)|

### Diving48

| 配置文件                                                     | GPU 数量 | 主干网络 |  预训练  | top1 准确率 | top5 准确率 | GPU 显存占用 (M) |                             ckpt                             |                             log                              |                             json                             |
| :----------------------------------------------------------- | :------: | :------: | :------: | :---------: | :---------: | :--------------: | :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
| [tsm_r50_video_1x1x8_50e_diving48_rgb](/configs/recognition/tsm/tsm_r50_video_1x1x8_50e_diving48_rgb.py) |    8     | ResNet50 | ImageNet |    75.99    |    97.16    |       7070       | [ckpt](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_video_1x1x8_50e_diving48_rgb/tsm_r50_video_1x1x8_50e_diving48_rgb_20210426-aba5aa3d.pth) | [log](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_video_1x1x8_50e_diving48_rgb/20210426_012424.log) | [json](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_video_1x1x8_50e_diving48_rgb/20210426_012424.log.json) |
| [tsm_r50_video_1x1x16_50e_diving48_rgb](/configs/recognition/tsm/tsm_r50_video_1x1x16_50e_diving48_rgb.py) |    8     | ResNet50 | ImageNet |    81.62    |    97.66    |       7070       | [ckpt](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_video_1x1x16_50e_diving48_rgb/tsm_r50_video_1x1x16_50e_diving48_rgb_20210426-aa9631c0.pth) | [log](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_video_1x1x16_50e_diving48_rgb/20210426_012823.log) | [json](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_video_1x1x16_50e_diving48_rgb/20210426_012823.log.json) |

### MixUp & CutMix on Something-Something V1

| 配置文件                                                      | 分辨率 | GPU 数量 | 主干网络 | 预训练 | top1 准确率 (efficient/accurate) | top5 准确率 (efficient/accurate) | top1 准确率变化 (efficient/accurate) | top5 准确率变化 (efficient/accurate) |                             ckpt                             |                             log                              |                             json                             |
| :----------------------------------------------------------- | :--------: | :--: | :------: | :------: | :---------------------------: | :---------------------------: | :---------------------------------: | :---------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
| [tsm_r50_mixup_1x1x8_50e_sthv1_rgb](/configs/recognition/tsm/tsm_r50_mixup_1x1x8_50e_sthv1_rgb.py) | 高 100 |  8   | ResNet50 | ImageNet |         46.35 / 48.49         |         75.07 / 76.88         |            +0.77 / +0.79            |            +0.05 / +0.70            | [ckpt](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_mixup_1x1x8_50e_sthv1_rgb/tsm_r50_mixup_1x1x8_50e_sthv1_rgb-9eca48e5.pth) | [log](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_mixup_1x1x8_50e_sthv1_rgb/tsm_r50_mixup_1x1x8_50e_sthv1_rgb.log) | [json](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_mixup_1x1x8_50e_sthv1_rgb/tsm_r50_mixup_1x1x8_50e_sthv1_rgb.json) |
| [tsm_r50_cutmix_1x1x8_50e_sthv1_rgb](/configs/recognition/tsm/tsm_r50_cutmix_1x1x8_50e_sthv1_rgb.py) | 高 100 |  8   | ResNet50 | ImageNet |         45.92 / 47.46         |         75.23 / 76.71         |            +0.34 / -0.24            |            +0.21 / +0.59            | [ckpt](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_cutmix_1x1x8_50e_sthv1_rgb/tsm_r50_cutmix_1x1x8_50e_sthv1_rgb-34934615.pth) | [log](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_cutmix_1x1x8_50e_sthv1_rgb/tsm_r50_cutmix_1x1x8_50e_sthv1_rgb.log) | [json](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_cutmix_1x1x8_50e_sthv1_rgb/tsm_r50_cutmix_1x1x8_50e_sthv1_rgb.json) |

### Jester

| 配置文件                                                     | 分辨率 | GPU 数量 | 主干网络 |  预训练  | top1 准确率 (efficient/accurate) |                             ckpt                             |                             log                              |                             json                             |
| ------------------------------------------------------------ | :----: | :------: | :------: | :------: | :------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
| [tsm_r50_1x1x8_50e_jester_rgb](/configs/recognition/tsm/tsm_r50_1x1x8_50e_jester_rgb.py) | 高 100 |    8     | ResNet50 | ImageNet |           96.5 / 97.2            | [ckpt](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_1x1x8_50e_jester_rgb/tsm_r50_1x1x8_50e_jester_rgb-c799267e.pth) | [log](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_1x1x8_50e_jester_rgb/tsm_r50_1x1x8_50e_jester_rgb.log) | [json](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_r50_1x1x8_50e_jester_rgb/tsm_r50_1x1x8_50e_jester_rgb.json) |

### HMDB51

| 配置文件                                                     | GPU 数量 | 主干网络 |   预训练    | top1 准确率 | top5 准确率 | GPU 显存占用 (M) |                             ckpt                             |                             log                              |                             json                             |
| :----------------------------------------------------------- | :------: | :------: | :---------: | :---------: | :---------: | :--------------: | :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
| [tsm_k400_pretrained_r50_1x1x8_25e_hmdb51_rgb](/configs/recognition/tsm/tsm_k400_pretrained_r50_1x1x8_25e_hmdb51_rgb.py) |    8     | ResNet50 | Kinetics400 |    72.68    |    92.03    |      10388       | [ckpt](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_k400_pretrained_r50_1x1x8_25e_hmdb51_rgb/tsm_k400_pretrained_r50_1x1x8_25e_hmdb51_rgb_20210630-10c74ee5.pth) | [log](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_k400_pretrained_r50_1x1x8_25e_hmdb51_rgb/20210605_182554.log) | [json](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_k400_pretrained_r50_1x1x8_25e_hmdb51_rgb/20210605_182554.log.json) |
| [tsm_k400_pretrained_r50_1x1x16_25e_hmdb51_rgb](/configs/recognition/tsm/tsm_k400_pretrained_r50_1x1x16_25e_hmdb51_rgb.py) |    8     | ResNet50 | Kinetics400 |    74.77    |    93.86    |      10388       | [ckpt](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_k400_pretrained_r50_1x1x16_25e_hmdb51_rgb/tsm_k400_pretrained_r50_1x1x16_25e_hmdb51_rgb_20210630-4785548e.pth) | [log](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_k400_pretrained_r50_1x1x16_25e_hmdb51_rgb/20210605_182505.log) | [json](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_k400_pretrained_r50_1x1x16_25e_hmdb51_rgb/20210605_182505.log.json) |

### UCF101

| 配置文件                                                     | GPU 数量 | 主干网络 |   预训练    | top1 准确率 | top5 准确率 | GPU 显存占用 (M) |                             ckpt                             |                             log                              |                             json                             |
| :----------------------------------------------------------- | :------: | :------: | :---------: | :---------: | :---------: | :--------------: | :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
| [tsm_k400_pretrained_r50_1x1x8_25e_ucf101_rgb](/configs/recognition/tsm/tsm_k400_pretrained_r50_1x1x8_25e_ucf101_rgb.py) |    8     | ResNet50 | Kinetics400 |    94.50    |    99.58    |      10389       | [ckpt](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_k400_pretrained_r50_1x1x8_25e_ucf101_rgb/tsm_k400_pretrained_r50_1x1x8_25e_ucf101_rgb_20210630-1fae312b.pth) | [log](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_k400_pretrained_r50_1x1x8_25e_ucf101_rgb/20210605_182720.log) | [json](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_k400_pretrained_r50_1x1x8_25e_ucf101_rgb/20210605_182720.log.json) |
| [tsm_k400_pretrained_r50_1x1x16_25e_ucf101_rgb](/configs/recognition/tsm/tsm_k400_pretrained_r50_1x1x16_25e_ucf101_rgb.py) |    8     | ResNet50 | Kinetics400 |    94.58    |    99.37    |      10389       | [ckpt](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_k400_pretrained_r50_1x1x16_25e_ucf101_rgb/tsm_k400_pretrained_r50_1x1x16_25e_ucf101_rgb_20210630-8df9c358.pth) | [log](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_k400_pretrained_r50_1x1x16_25e_ucf101_rgb/20210605_182720.log) | [json](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_k400_pretrained_r50_1x1x16_25e_ucf101_rgb/20210605_182720.log.json) |

注：

1. 这里的 **GPU 数量** 指的是得到模型权重文件对应的 GPU 个数。默认地，MMAction2 所提供的配置文件对应使用 8 块 GPU 进行训练的情况。
   依据 [线性缩放规则](https://arxiv.org/abs/1706.02677)，当用户使用不同数量的 GPU 或者每块 GPU 处理不同视频个数时，需要根据批大小等比例地调节学习率。
   如，lr=0.01 对应 4 GPUs x 2 video/gpu，以及 lr=0.08 对应 16 GPUs x 4 video/gpu。
2. 这里的 **推理时间** 是根据 [基准测试脚本](/tools/analysis/benchmark.py) 获得的，采用测试时的采帧策略，且只考虑模型的推理时间，
   并不包括 IO 时间以及预处理时间。对于每个配置，MMAction2 使用 1 块 GPU 并设置批大小（每块 GPU 处理的视频个数）为 1 来计算推理时间。
3. 参考代码的结果是通过使用相同的模型配置在原来的代码库上训练得到的。对应的模型权重文件可从 [这里](https://download.openmmlab.com/mmaction/recognition/tsm/tsm_reference_ckpt.rar) 下载。
4. 对于 Something-Something 数据集，有两种测试方案：efficient（对应 center crop x 1 clip）和 accurate（对应 Three crop x 2 clip）。两种方案参考自 [原始代码库](https://github.com/mit-han-lab/temporal-shift-module/tree/8d53d6fda40bea2f1b37a6095279c4b454d672bd)。
   MMAction2 使用 efficient 方案作为配置文件中的默认选择，用户可以通过以下方式转变为 accurate 方案：

```python
...
test_pipeline = [
    dict(
        type='SampleFrames',
        clip_len=1,
        frame_interval=1,
        num_clips=16,   # 当使用 8 个 视频段时，设置 `num_clips = 8`
        twice_sample=True,    # 设置 `twice_sample=True` 用于 accurate 方案中的 Twice Sample
        test_mode=True),
    dict(type='RawFrameDecode'),
    dict(type='Resize', scale=(-1, 256)),
    # dict(type='CenterCrop', crop_size=224), 用于 efficient 方案
    dict(type='ThreeCrop', crop_size=256),  # 用于 accurate 方案
    dict(type='Normalize', **img_norm_cfg),
    dict(type='FormatShape', input_format='NCHW'),
    dict(type='Collect', keys=['imgs', 'label'], meta_keys=[]),
    dict(type='ToTensor', keys=['imgs'])
]
```

5. 当采用 Mixup 和 CutMix 的数据增强时，使用超参 `alpha=0.2`。
6. 我们使用的 Kinetics400 验证集包含 19796 个视频，用户可以从 [验证集视频](https://mycuhk-my.sharepoint.com/:u:/g/personal/1155136485_link_cuhk_edu_hk/EbXw2WX94J1Hunyt3MWNDJUBz-nHvQYhO9pvKqm6g39PMA?e=a9QldB) 下载这些视频。同时也提供了对应的 [数据列表](https://download.openmmlab.com/mmaction/dataset/k400_val/kinetics_val_list.txt) （每行格式为：视频 ID，视频帧数目，类别序号）以及 [标签映射](https://download.openmmlab.com/mmaction/dataset/k400_val/kinetics_class2ind.txt) （类别序号到类别名称）。
7. 这里的 **infer_ckpt** 表示该模型权重文件是从 [TSM](https://github.com/mit-han-lab/temporal-shift-module/blob/master/test_models.py) 导入的。

对于数据集准备的细节，用户可参考 [数据集准备文档](/docs/zh_cn/data_preparation.md) 中的 Kinetics400, Something-Something V1 and Something-Something V2 部分。

## 如何训练

用户可以使用以下指令进行模型训练。

```shell
python tools/train.py ${CONFIG_FILE} [optional arguments]
```

例如：以一个确定性的训练方式，辅以定期的验证过程进行 TSM 模型在 Kinetics-400 数据集上的训练。

```shell
python tools/train.py configs/recognition/tsm/tsm_r50_1x1x8_50e_kinetics400_rgb.py \
    --work-dir work_dirs/tsm_r50_1x1x8_100e_kinetics400_rgb \
    --validate --seed 0 --deterministic
```

更多训练细节，可参考 [基础教程](/docs/zh_cn/getting_started.md#训练配置) 中的 **训练配置** 部分。

## 如何测试

用户可以使用以下指令进行模型测试。

```shell
python tools/test.py ${CONFIG_FILE} ${CHECKPOINT_FILE} [optional arguments]
```

例如：在 Kinetics-400 数据集上测试 TSM 模型，并将结果导出为一个 json 文件。

```shell
python tools/test.py configs/recognition/tsm/tsm_r50_1x1x8_50e_kinetics400_rgb.py \
    checkpoints/SOME_CHECKPOINT.pth --eval top_k_accuracy mean_class_accuracy \
    --out result.json
```

更多测试细节，可参考 [基础教程](/docs/zh_cn/getting_started.md#测试某个数据集) 中的 **测试某个数据集** 部分。
