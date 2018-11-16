# dataset-action-2

This dataset was recorded from the standalone realsense camera.
In each dataset, the subject is steady for the first seconds, in order to allow the `skeletonRetriever` to observe the skeleton and perform the optimization. 

The train folder contains 50 subfolders, each containing 10 repetitions of a single action. Each action is repeated 5 times and viewed from 2 points of view.
The test folder contains 5 subfolders, each containing 10 repetitions of a single action, viewed from a single point of view.

Points of view are named as following:
* v0: frontal view
* v1: side view

Actions are named as following:
* abduction-left
* external-left
* internal-left
* random (for random movements)
* static (for no movements)
 
Each folder is named as **person name-point of view - action name**, containing the following subfolders:
* depth: stores depth images 
* skeletons-data: stores skeletons bottles
* skeletons-img: stores skeletons images
* opc: stores skeletons from opc
* opc-optimized: stores skeletons from opc after the optimization
