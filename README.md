# 3DReconstruction_Gaussian-Splatting
3D Scene Reconstruction Based on SLAM and 3D Gaussian Splatting

# 3D_Recon_SLAM_ws

- Ubuntu 20.04
- NVIDIA Jetson Orin Nano 4G

# Getting Started
## GS-SLAM 环境配置

Setup the environment.
```
conda env create -f environment.yml
conda activate MonoGS
```
## rosbag to rgbd
Data path : datasets/tum
```bash
python convert.py
``` 

## Training
```bash
CUDA_VISIBLE_DEVICES=0 python slam.py --config configs/rgbd/tum/rosBag7.yaml 
```

