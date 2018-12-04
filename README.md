# assistive-rehab-storage
Storage repository for Assistive and Rehabilitative Robotics.

Use [Git LFS](https://git-lfs.github.com) to archive/download files.

## Repository structure
The assistive-rehab-storage repository contains the following directories:
1. `dataset-action-1`: recorded from r1-mk2, containing 4 classes. More details can be found [following link](README_dataset1.md). 
2. `dataset-action-2`: recorded from realsense, containing 6 classes (same as `dataset-action-1` plus the classes `reaching-left` and `static`). In each dataset, the subject is initially steady for few seconds, in order to let the `skeletonRetriever` observe the skeleton and optimize it. More details can be found [following link](README_dataset2.md).
