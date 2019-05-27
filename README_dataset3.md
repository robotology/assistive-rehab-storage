# dataset-action-3

This dataset was recorded from the standalone r1-mk2.
In each dataset, the subject is steady for the first seconds, in order to allow the `skeletonRetriever` to observe the skeleton and perform the optimization.

The train folder contains 38 subfolders, each containing 10 repetitions of a single action. Each action, except the reaching, is repeated 5 times and viewed from 2 points of view. The reaching action is performed in order to reach 4 different targets, distributed on the corners/center of a square, centered around the `shoulderCenter` of the subject.

Points of view are named as following:
* v0: frontal view
* v1: side view

Actions are named as following:
* abduction-right
* external-right
* internal-right
* reaching-right

For the reaching-left action, targets to be reached are distributed in a square, and are specified as following:
* t1: target in the center of the square  
* t2: target in the top-right corner
* t3: target in the bottom-right corner
* t4: target in the bottom-left corner

Each folder is named as **person name-point of view-target - action name** (target is specified only for the reaching action), containing the following subfolders:
* depth: stores depth images
* skeletons-data: stores skeletons bottles
* skeletons-img: stores skeletons images
* opc: stores skeletons from opc
* opc-optimized: stores skeletons from opc after the optimization at three different speeds, obtained by changing the twarp parameter in the [skeletonPlayer](https://robotology.github.io/assistive-rehab/doc/doxygen/doc/html/classskeletonPlayer__IDL.html):
    - twarp=0: speed of acquisition;
    - twarp=0.3: squeezed original stream (higher speed);
    - twarp=1.5: dilated original stream (lower speed).
