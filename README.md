# unknown-yolo


### 不同风格图像与视频对比展示
|Model                |Yolov5x |unknown-Yolov5x |
|---                  |---  |---  
|电影                 |![image](https://user-images.githubusercontent.com/84908793/167085804-5c09d3fc-86d4-4cee-9332-022df4893c00.png) |![image](https://user-images.githubusercontent.com/84908793/167085875-ea95cab2-6ed5-42d2-a46e-bd118c61275c.png)
|游戏                 |![image](https://user-images.githubusercontent.com/84908793/167086513-7473fb8a-efb2-4c9f-9f65-98b8bbe2da90.png) |![image](https://user-images.githubusercontent.com/84908793/167086544-ada61b28-2d27-4d76-ae7c-ddae466e5f96.png)
|漫画                 |![image](https://user-images.githubusercontent.com/84908793/167086664-c07f3e3b-d6f3-4261-8333-912886eb3d20.png) |![image](https://user-images.githubusercontent.com/84908793/167086687-eaace9c4-71be-4f12-bbe4-5a0a80725529.png)

|动漫                 |![image](https://user-images.githubusercontent.com/84908793/167086743-a73c0352-e0e5-45d6-9246-afed20c13d9b.png) |![image](https://user-images.githubusercontent.com/84908793/167086764-3236c5c0-7dc0-4d9e-89be-10b6b4bc8edd.png)



<br>![image](https://user-images.githubusercontent.com/84908793/162931434-dc4da5c4-7916-4cee-af1c-a2f1037d1bf1.png)<br><br>
简介：<br>
不增加推理训练成本，使yolov5-6.0涨点的同时具有一定程度检测未知物体的能力，代码大概今年毕业后开源。<br>
网络结构未发生变化，仅增加了一个分类（80—81）和修改损失函数。下表为初代版本实验结果对比。

Introduction:<br>
Without increasing the cost of reasoning training, the map of yolov5-6.0 is slightly improved and has the ability to detect unknown objects to a certain extent. The code will be open source after graduation this year.<br>
The network structure has not changed, only a classification (80-81) is added and the loss function is modified.
The following table shows the comparison of experimental results of the first generation version.

### 主要技术
luck<br>
sls

### coco数据集
|Model |size<br><sup>(pixels) |batch |mAP<sup>val<br>0.5:0.95 |mAP<sup>val<br>0.5 |
|---                  |---  |---    |---    |---   
|YOLOv5s              |640  |128    |37.4   |56.8  
|unknown-YOLOv5s      |640  |64     |37.5   |56.8
|YOLOv5x              |640  |64    |50.7   |68.9   
|unknown-YOLOv5x      |640  |64     |50.9   |69.3     

### voc数据集
|Model |size<br><sup>(pixels) |mAP<sup>val<br>0.5:0.95 |mAP<sup>val<br>0.5 |pre(coco)
|---                        |---  |---    |---       |---   
|YOLOv5s                    |512  |62.4   |86.7      |5s
|unknown-YOLOv5s            |512  |62.4   |86.8      |un-5s 
|YOLOv5x                    |512  |74.6   |91.9/92.1 |5x
|unknown-YOLOv5x            |512  |74.7   |92.2      |un-5

### 预训练模型和示例图像下载地址
  [unknown-yolov5s](https://github.com/buxihuo/unknown-yolo/releases/download/unknown-yolo/unknown-yolov5s.pt)<br>
  [unknown-yolov5x](https://github.com/buxihuo/unknown-yolo/releases/download/unknown-yolo/unknown-yolov5x.pt)<br>
  [images.zip](https://github.com/buxihuo/unknown-yolo/releases/download/unknown-yolo/images.zip)<br>
