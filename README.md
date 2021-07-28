## Tracking algorithm

### Python Environment Setup
1) Use the provided `env.yml` to install required dependencies <br>
2) Run `conda env install -f env.yml` <br>
3) Add `export PYTHONPATH=$PYTHONPATH:/path_to_root` to `~/.bashrc` <br>


### Using the algorithm
1) The algorithm requires calibration files based on the location of the cameras. <br>
2) The tracking algorithm can be used to either extract or replay trajectories from the video 
3) To extract tracking data in `*.npy` format, use `tracking.py` with `replay=False`, `save=True`(save logs)
4) The video and calibration files are to be placed in a folder parent to the root_folder
5) Sample [video](https://drive.google.com/drive/folders/1TQiYoiA1uMNZHRfJPVhJXa6p-TgNV2PX?usp=sharing) and [calibration files](https://drive.google.com/file/d/1Pll2jAHzyQONjZ6ThRXL4I-WMVeCfhN7/view?usp=sharing) are provided.

### Expected folder structure
- /
- /avacar_data/video (raw_videos to be put here)
- /avacar_data/processed_video (output video to visualize tracking results)
- /avacar_data/calibration_2d (config files here)
- /avacar_data/tracking (folder to save all the log files created by algo)
- /tracking_3d (tracker code)
  

### References

If you find this alogorithm useful for your work, please cite it as follows: <br>

  <a href="https://arxiv.org/abs/2104.00893"> Duo Lu, Varun C Jammula, Steven Como, Jeffrey Wishart, Yan Chen, & Yezhou Yang. (2021). CAROM – Vehicle Localization and Traffic Scene Reconstruction from Monocular Cameras on Road Infrastructures. </a>
