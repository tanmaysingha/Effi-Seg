# Effi-Seg: Rethinking EfficientNet Architecture for Real-time Semantic Segmentation 
This is an official site for Effi-Seg model. Currently, the model predictions and supplimentary materials are uploaded. Upon the acceptance of the paper, this repository will be updated.

## Datasets
For this research work, we used three different datasets for urban street scene analysis for outdoor and indoor scene analysis.
# Outdoor datasets:
* Cityscapes - To access this benchmark, user needs an account. For test set evaluation, user needs to upload all the test set results into the server. https://www.cityscapes-dataset.com/downloads/ 
* BDD100K - To access this benchmark, user needs an account. Here is the link for this dataset: https://doc.bdd100k.com/download.html#k-images
* KITTI - To access this benchmark, user needs an account. Like Cityscapes, user needs to submit the test set result to the evaluation server.  http://www.cvlibs.net/datasets/kitti/eval_semseg.php?benchmark=semantics2015    

Notes: All these three datasets are 
## Metrics
To understand the metrics used for model performance evaluation, please  refer here: https://www.cityscapes-dataset.com/benchmarks/#pixel-level-results

## Results
We trained our model by the above mentioned benchmarks at different input resolutions. For Cityscapes and KITTI datasets, we use 19 classes, however for Camvid dataset we trained the model with 11 classes (suggested by the literature). The following table exhibits the test results achieved by SDBNet.

Dataset    | No. of classes  | Input Size  |  Val/Test mIoU  | No. of parameters | FPS   
-----------|-----------------|-------------|-----------------|-------------------|--------
Cityscapes |        19       | 1024 * 2048 |  69.3% (test)   |    1.49 million   | 188
BDD100K    |        19       |  768 * 1280 |  54.9%  (val)   |    1.49 million   | 103
KITTI      |        19       |  384 * 1280 |  56.2% (test)   |    1.49 million   | 201

Notes: Model Effi-Seg has 8.4G FLOPs at 512 * 1024 input resolution.

### Cityscapes test results
The output of the test set is submitted to Cityscapes evaluation server. To view the test set result evaluated by the server, click the following link: https://www.cityscapes-dataset.com/anonymous-results/?id=4d35fe35555ed7b145ebcaaa6d45275b5ea3e1a18c6cf43734a8d7bde6495224
This is an anonymous link given by the Cityscapes server. Upon the acceptance of the paper, test result will be cited by the paper and will be published in the evaluation server.

### KITTI test set results
Like Cityscapes, KITTI test set result is also sumbitted to the evaluation server. Click the following link to see the result:
https://github.com/tanmaysingha/SDBNetV2/blob/main/other_files/best_results_KITTI_mIoU.pdf

### Color map of Cityscapes dataset and model prediction using validation sample
![cityscapes_val_set](https://github.com/tanmaysingha/SDBNetV2/blob/main/Figures/City_color_map.png?raw=true)  

### Color map of CamVid dataset and model prediction using validation sample
![CamVid_val_set](https://github.com/tanmaysingha/SDBNetV2/blob/main/Figures/camvid_color_map.png?raw=true)

### Color map of IDD-lite dataset and model prediction using validation sample
![IDDLite_val_set](https://github.com/tanmaysingha/SDBNetV2/blob/main/Figures/color_map_IDD.png?raw=true)

### Color map of Indoor objects dataset and model prediction using validation sample
![Indoor_val_set](https://github.com/tanmaysingha/SDBNetV2/blob/main/Figures/color_map_indoor.png?raw=true)

### SDBNetV2 prediction on Cityscapes test samples
![Cityscapes_test_set](https://github.com/tanmaysingha/SDBNetV2/blob/main/Figures/city_test_pred.png?raw=true)

### SDBNetV2 prediction on BDD100K test samples
![BDD100K_test_set](https://github.com/tanmaysingha/SDBNetV2/blob/main/Figures/BDD_test_pred.png?raw=true)

### SDBNetV2 prediction on CamVid validation sample
![CamVid_val_set](https://github.com/tanmaysingha/SDBNetV2/blob/main/Figures/fig_CamVid_test.png?raw=true)

### SDBNetV2 prediction on KITTI test samples
![KITTI_test_set](https://github.com/tanmaysingha/SDBNetV2/blob/main/Figures/fig_KITTI_test.png?raw=true)

### SDBNetV2 prediction on IDD-lite validation samples
![IDDLite_test_set](https://github.com/tanmaysingha/SDBNetV2/blob/main/Figures/Idd_lite_test_pred.png?raw=true)

### SDBNetV2 prediction on IDD (part1 and part2) and Cityscapes validation samples
![IDD_City_test_set](https://github.com/tanmaysingha/SDBNetV2/blob/main/Figures/IDD_Cityscapes_1ID_pred.png?raw=true)
