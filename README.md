# 简介（Introduction）<br>
赋予检测器初步认知能力，区分已知与未知物体，已实现的检测器有:yolov5
```bash
'''
此为新版本，正在合并用于测试和推理的参数，即将完成，旧版见OW-yolov5-6.0分支。
'''
```

# 使用方法（Usage）
<br>

![屏幕截图 2022-07-06 234014](https://user-images.githubusercontent.com/84908793/177590154-9956552a-3f5b-43a1-9598-9d980eb41fcf.jpg)

<details>
<summary>Usage 1</summary>
 
</details>

<details open>
<summary>Usage 2</summary>

</details>

<details>
<summary>Usage 3</summary>
 
</details>
<br>

# 快速开始

## 1. 安装

## 2. 推理

## 3. 测试

## 4. 训练

# 性能（performance）

## 1. 精度曲线（precision curve）

![下载 (5)](https://user-images.githubusercontent.com/84908793/177591053-a083a20c-6fed-4beb-aff5-80e0e54bace5.png)

<details>
<summary>说明</summary>
 
```bash
   模型在coco(80类)数据集训练，在object365(365类)进行测试,将coco上对应的类作为已知类，其他的作为未知类。其中灰色是已知类别的精度曲线，
   红色为未知类别精度曲线，蓝色代表所有    类别的平均值。
```
 
</details>

## 2. 召回率曲线（recall curve）

![下载 (6)](https://user-images.githubusercontent.com/84908793/177591425-b226222c-56b1-4036-9d0a-ed5aaab31f4e.png)

## 3. map

### 1) coco数据集性能对比

|Model                        |Param |Flops  |mAP<sup>val<br>0.5:0.95 |mAP<sup>val<br>0.5 
|---                          |---   |---    |---                     |---   
|Detr                         |34    |78     |39. 4                   |-
|OW-detr                      |-     |-      |33.1(-6.3)              |-  
|yolov5s                      |      |       |38.46                   |56.8  
|OW-yolov5s(only known)       |      |       |38.46                   |57.16
|OW-yolov5s<br>(unknown background confidence = 0.001)      |      |       |37.36                 |54.82
|OW-yolov5s<br>(unknown background confidence = 0.01)       |      |       |38.29                 |56.80
|OW-yolov5s<br>(unknown background confidence = 0.05)       |      |       |38.42                 |57.09
|OW-yolov5s<br>(unknown background confidence = 0.1)        |      |       |38.44                 |57.14
|OW-yolov5s<br>(unknown background confidence = 0.25)       |      |       |38.45                 |57.16
|OW-yolov5s<br>(unknown background confidence = 0.5)        |      |       |38.46                 |57.17



### 2) object365 数据集

|Model                                                      |unknown recall |unknown ap50  |all mAP<sup>val<br>0.5:0.95 |all mAP<sup><br>0.5 
|---                                                        |---            |---           |---                         |---   
|yolov5s                                                    |       -       |   -          |                            |
|OW-yolov5s(only known)                                     |       -       |   -          |                            |
|OW-yolov5s<br>(unknown background confidence = 0.001)      |               |              |                            |
|OW-yolov5s<br>(unknown background confidence = 0.01)       |               |              |                            |
|OW-yolov5s<br>(unknown background confidence = 0.05)       |               |              |                            | 
|OW-yolov5s<br>(unknown background confidence = 0.1)        |0.23               |12.3              |22.2                            |32.3
|OW-yolov5s<br>(unknown background confidence = 0.25)       |0.15               |13.5              |22.2                            |32.3
|OW-yolov5s<br>(unknown background confidence = 0.5)        |0.08               |13.5              |22.2                            |32.3


### 3) 其他版本

