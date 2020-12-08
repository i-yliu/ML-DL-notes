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
  * AP: average precision; Area under the precision-recall cruve (PR curve) with different threshold.
  * ![PRcurve](https://miro.medium.com/max/600/0*IIP5_lTXigXMViiu.png)
    
  * IoU: area of overlap / area of union -> Both for bounding boxes and segmentation masks.
  * AP@ RANEGE \[0.5: 0.95] 
  * mAP[https://medium.com/@yanfengliux/the-confusing-metrics-of-ap-and-map-for-object-detection-3113ba0386ef]: Mean average precision (mAP). All AP values averaged over different classes/categories.
  * ROC curve: y-TP rate x-FN rate | y-precision x-1-sepcificicity (tn / negatives)
  
* Evaluation metic for object detection/instance segmentation
  * ![PRcurve](https://img-blog.csdnimg.cn/20190225102148830.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2xpbmd6aG91MzM=,size_16,color_FFFFFF,t_70)

