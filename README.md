# unknown-yolo
简介：<br>
不增加推理训练成本，使yolov5-6.0涨点的同时具有一定程度检测未知物体的能力，代码大概今年毕业后开源。<br>
网络结构未发生变化，仅增加了一个分类（80—81）和修改损失函数。

Introduction:<br>
Without increasing the cost of reasoning training, the map of yolov5-6.0 is slightly improved and has the ability to detect unknown objects to a certain extent. The code will be open source after graduation this year.<br>
The network structure has not changed, only a classification (80-81) is added and the loss function is modified.

### 不同风格图像与视频对比展示
|Model                |Yolov5x |unknown-Yolov5x |
|---                  |---  |---  
|漫画                 |![图片 46](https://user-images.githubusercontent.com/84908793/167087540-c109830f-3a0c-42d6-8948-61c96a3925aa.png) |![图片 47](https://user-images.githubusercontent.com/84908793/167087925-5332b077-9481-44a4-af93-0c1c4e175ff1.png)
|电影                 |![图片 43](https://user-images.githubusercontent.com/84908793/167087873-bcba6a22-9798-4d51-b9f5-b610c8fe1a51.png) |![图片 37](https://user-images.githubusercontent.com/84908793/167087888-e4749d62-4bec-47ab-b235-9dcd45cd5440.png)
|游戏                 |![图片 2](https://user-images.githubusercontent.com/84908793/167087802-40ef99d0-2658-444a-b02f-df258e1538b1.png)  |![图片 1](https://user-images.githubusercontent.com/84908793/167087825-98c33a0c-4345-4f51-bb2e-6fe7bd96b182.png)
|动漫                 |![图片 4](https://user-images.githubusercontent.com/84908793/167087943-bd4179c6-0f24-4721-810d-deb3e17b8eed.png)  |![图片 3](https://user-images.githubusercontent.com/84908793/167087955-18f042b2-5658-40e6-99fb-f43562051ebe.png)

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
  
<br>![image](https://user-images.githubusercontent.com/84908793/162931434-dc4da5c4-7916-4cee-af1c-a2f1037d1bf1.png)<br><br>

### 预训练模型和示例图像下载地址
  [unknown-yolov5s](https://github.com/buxihuo/unknown-yolo/releases/download/unknown-yolo/unknown-yolov5s.pt)<br>
  [unknown-yolov5x](https://github.com/buxihuo/unknown-yolo/releases/download/unknown-yolo/unknown-yolov5x.pt)<br>
  [images.zip](https://github.com/buxihuo/unknown-yolo/releases/download/unknown-yolo/images.zip)<br>
