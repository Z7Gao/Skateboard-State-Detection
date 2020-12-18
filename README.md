# Skateboard
Computer Vision 2020 Course Project


openpose[CMU]:https://github.com/CMU-Perceptual-Computing-Lab/openpose



## TODO

- 高子淇：跑通openpose
- 赵乘风：跑通openpose，整理数据集
- 李德润：搜集平面与物体关系检测的相关方法
- 刘芊渝：探索糊不糊方法
- 张晨杨：OpenCV 物体检测（coco dataset）



## Dev log

### Ziqi's part

### 12/12

- Running openpose successfully;

- Uploading the result on reduced dataset in `pose` , with json and jpg format for each image.


### 12/16

- Parse json files from openpose;

- Calculate 4 Angles and show the result.

### 12/18

- Process pose data into a csv file, with label mapping being { 0:flying, 1:sliding, 2:static}

- Testing multi-class classification using SVM on COCO dataset 

  |                                           | linear svc | rbf svc |
  | ----------------------------------------- | ---------- | ------- |
  | 3 classes, 100 imgs for each class        | ~0.60      | ~0.3    |
  | 2 classes (flying T/F), 200 imgs for each | ~0.75      | ~0.5    |

- Question: rbf overfit????

- 3 classes:

![image-20201219013551188](C:\Users\zwm\AppData\Roaming\Typora\typora-user-images\image-20201219013551188.png)

- 2 classes: 

![image-20201219013625406](C:\Users\zwm\AppData\Roaming\Typora\typora-user-images\image-20201219013625406.png)

