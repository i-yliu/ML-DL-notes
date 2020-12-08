* FPN
  * Top down bottom up, skip connection
  * Feature fusion element-wise add
  * Eech Level/scale has an output branch, which covers objects with different scales, and can increase the recall

* U-Net
  * U-Net and FPN have a very similar structure: both multiscale feature map fusion. High level feature fuse with low level feature.
  * Difference, U-net concatenation, FPN element-wise addition. U-net only output pixel level segmentation at last layer while FPN output prediction at each level.
  
* CNN

* Evaluation metic for object detection/instance segmentation
  * Precision: tp/(tp + fp); tp / predicted positive
  * Recall: tp/(tp+fn); tp / all positive
  * AP: average precision; Area under the precision-recall cruve(PR curve)
    ![PRcurve](https://miro.medium.com/max/600/0*IIP5_lTXigXMViiu.png)
