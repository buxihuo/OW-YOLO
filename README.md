### 简介（Introduction）<br>
无代价涨点 + 检测未知物体<br>

<br>![image](https://user-images.githubusercontent.com/84908793/162931434-dc4da5c4-7916-4cee-af1c-a2f1037d1bf1.png)<br><br>

### 不同风格图像与视频对比展示
|Model                |Yolov5x |Luck-Yolov5x |
|---                  |---  |---  
|漫画                 |![图片 46](https://user-images.githubusercontent.com/84908793/167087540-c109830f-3a0c-42d6-8948-61c96a3925aa.png) |![图片 47](https://user-images.githubusercontent.com/84908793/167087925-5332b077-9481-44a4-af93-0c1c4e175ff1.png)
|电影                 |![图片 43](https://user-images.githubusercontent.com/84908793/167087873-bcba6a22-9798-4d51-b9f5-b610c8fe1a51.png) |![图片 37](https://user-images.githubusercontent.com/84908793/167087888-e4749d62-4bec-47ab-b235-9dcd45cd5440.png)
|游戏                 |![图片 2](https://user-images.githubusercontent.com/84908793/167087802-40ef99d0-2658-444a-b02f-df258e1538b1.png)  |![图片 1](https://user-images.githubusercontent.com/84908793/167087825-98c33a0c-4345-4f51-bb2e-6fe7bd96b182.png)
|动漫                 |![图片 4](https://user-images.githubusercontent.com/84908793/167087943-bd4179c6-0f24-4721-810d-deb3e17b8eed.png)  |![图片 3](https://user-images.githubusercontent.com/84908793/167087955-18f042b2-5658-40e6-99fb-f43562051ebe.png)


### coco数据集
|Model |size<br><sup>(pixels) |batch |mAP<sup>val<br>0.5:0.95 |mAP<sup>val<br>0.5 |
|---                  |---  |---    |---    |---   
|YOLOv5s              |640  |128    |37.4   |56.8  
|Luck-YOLOv5s      |640  |64     |37.5   |56.8
|YOLOv5x              |640  |64    |50.7   |68.9   
|Luck-YOLOv5x      |640  |64     |50.9   |69.3     

### voc数据集
|Model |size<br><sup>(pixels) |mAP<sup>val<br>0.5:0.95 |mAP<sup>val<br>0.5 |pre(coco)
|---                        |---  |---    |---       |---   
|YOLOv5s                    |512  |62.4   |86.7      |5s
|Luck-YOLOv5s            |512  |62.4   |86.8      |un-5s 
|YOLOv5x                    |512  |74.6   |91.9/92.1 |5x
|Luck-YOLOv5x            |512  |74.7   |92.2      |un-5

### 预训练模型
  [Luck-yolov5s](https://github.com/buxihuo/unknown-yolo/releases/download/unknown-yolo/Luck-yolov5s.pt)<br>
  [Luck-yolov5x](https://github.com/buxihuo/unknown-yolo/releases/download/unknown-yolo/Luck-yolov5x.pt)<br>
