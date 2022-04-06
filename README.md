# unknown-yolo
简介：不增加推理训练成本，使yolov5-6.0涨点的同时具有一定程度检测未知物体的能力，代码即将开源。
      涨点还有很大的潜力，正在改进，下表为初代版本实验结果对比。

### coco数据集
|Model |size<br><sup>(pixels) |batch |mAP<sup>val<br>0.5:0.95 |mAP<sup>val<br>0.5 |
|---                  |---  |---    |---    |---   
|YOLOv5s              |640  |128    |37.4   |56.8  
|unknown-YOLOv5s      |640  |64     |数值稍后 |
|YOLOv5x              |640  |128    |50.7   |68.9   
|unknown-YOLOv5x      |640  |64     |50.9   |69.3        
  
### voc数据集
|Model |size<br><sup>(pixels) |mAP<sup>val<br>0.5:0.95 |mAP<sup>val<br>0.5 |
|---                  |---  |---    |---    
|YOLOv5s              |512  |62.4   |86.7 
|unknown-YOLOv5s      |512  |62.4   |86.8 
|YOLOv5x              |512  |74.6   |91.9/92.1   
|unknown-YOLOv5x      |512  |74.7   |92.2        

### 检测示例
![000000022396](https://user-images.githubusercontent.com/84908793/160353223-21156bd7-523d-4087-b9ad-1a5795ce33b0.jpg)
