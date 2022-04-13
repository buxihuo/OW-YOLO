# unknown-yolo
<br>![image](https://user-images.githubusercontent.com/84908793/162931434-dc4da5c4-7916-4cee-af1c-a2f1037d1bf1.png)<br><br>
简介：<br>
不增加推理训练成本，使yolov5-6.0涨点的同时具有一定程度检测未知物体的能力，代码大概今年毕业后开源。<br>
网络结构未发生变化，仅增加了一个分类（80—81）和修改损失函数。下表为初代版本实验结果对比。

Introduction:<br>
Without increasing the cost of reasoning training, the map of yolov5-6.0 is slightly improved and has the ability to detect unknown objects to a certain extent. The code will be open source after graduation this year.<br>
The network structure has not changed, only a classification (80-81) is added and the loss function is modified.
The following table shows the comparison of experimental results of the first generation version.

### 主要技术
luck：learn uncorrect and confusing knowledge 学习不正确的混淆的知识
sls: self lable smoothing 自标签平滑（实验中）

### coco数据集
|Model |size<br><sup>(pixels) |batch |mAP<sup>val<br>0.5:0.95 |mAP<sup>val<br>0.5 |
|---                  |---  |---    |---    |---   
|YOLOv5s              |640  |128    |37.4   |56.8  
|unknown-YOLOv5s      |640  |64     |37.5   |56.8
|YOLOv5x              |640  |128    |50.7   |68.9   
|unknown-YOLOv5x      |640  |64     |50.9   |69.3     

### voc数据集
|Model |size<br><sup>(pixels) |mAP<sup>val<br>0.5:0.95 |mAP<sup>val<br>0.5 |
|---                  |---  |---    |---    
|YOLOv5s              |512  |62.4   |86.7 
|unknown-YOLOv5s      |512  |62.4   |86.8 
|YOLOv5x              |512  |74.6   |91.9/92.1   
|unknown-YOLOv5x      |512  |74.7   |92.2        

### 预训练模型和示例图像下载地址
  [unknown-yolov5s](https://github.com/buxihuo/unknown-yolo/releases/download/unknown-yolo/unknown-yolov5s.pt)<br>
  [unknown-yolov5x](https://github.com/buxihuo/unknown-yolo/releases/download/unknown-yolo/unknown-yolov5x.pt)<br>
  [images.zip](https://github.com/buxihuo/unknown-yolo/releases/download/unknown-yolo/images.zip)<br>
