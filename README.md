# Effi-Seg: Rethinking EfficientNet Architecture for Real-time Semantic Segmentation 
This is an official site for Effi-Seg model. Currently, the model predictions and supplimentary materials are uploaded. Upon the acceptance of the paper, this repository will be updated.

## Datasets
To evaluate model's performance, we used three different datasets the following three datasets:
* Cityscapes - To access this benchmark, user needs an account. For test set evaluation, user needs to upload all the test set results into the server. https://www.cityscapes-dataset.com/downloads/ 
* BDD100K - To access this benchmark, user needs an account. Here is the link for this dataset: https://doc.bdd100k.com/download.html#k-images
* KITTI - To access this benchmark, user needs an account. Like Cityscapes, user needs to submit the test set result to the evaluation server.  http://www.cvlibs.net/datasets/kitti/eval_semseg.php?benchmark=semantics2015    

Notes: The classes of KITTI and BDD100K datasets are compatiable with Cityscapes dataset. Hence, We used 19 classes for model's performance evaluation on all three datasets.

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
The output of the test set is submitted to Cityscapes evaluation server. To view the test set result evaluated by the server, click the following link: 
https://www.cityscapes-dataset.com/anonymous-results/?id=07a774c5792e9fbceefa8bdd207cce4816f26b523f9c359cef72b0cf36119ffa
This is an anonymous link given by the Cityscapes server. Upon the acceptance of the paper, test result will be cited by the paper and will be published in the evaluation server.
We also uploaded the printed pdf copy in our repository. Here is the link:
https://github.com/tanmaysingha/Effi-Seg/blob/main/other_files/Cityscapes_test_results.pdf

### KITTI test set results
Like Cityscapes, KITTI test set result is also sumbitted to the evaluation server. Click the following link to see the result:
https://github.com/tanmaysingha/Effi-Seg/blob/main/other_files/KITTI_test_results.pdf

### Color map of all three datasets
![cityscapes_val_set](https://github.com/tanmaysingha/Effi-Seg/blob/main/Figures/colors_map.png?raw=true)  

### Effi-Seg prediction using Cityscapes validation and test samples
![Cityscapes_test_set](https://github.com/tanmaysingha/Effi-Seg/blob/main/Figures/Cityscapes_prediction.png?raw=true)

### Effi-Seg prediction using BDD100K validation and test samples
![BDD100K_test_set](https://github.com/tanmaysingha/Effi-Seg/blob/main/Figures/BDD_prediction.png?raw=true)

### Effi-Seg prediction using KITTI validation and test samples
![KITTI_test_set](https://github.com/tanmaysingha/Effi-Seg/blob/main/Figures/KITTI_prediction.png?raw=true)
