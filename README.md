![015](https://user-images.githubusercontent.com/84908793/221391769-2503d415-60c3-4c4b-a432-a4f0fdfa186c.png)

# 快速开始

## 1. 安装
  同yolov5

## 2. 推理

<details> 
<summary> 推理示例</summary>

```bash
$ python detect.py --source data/images --weights m-obj365.pt --unknownconf 0.45 --conf 0.25 
$ python detect.py --source data/images --weights s-coco.pt --unknownconf 0.25 --conf 0.25
'''
参数解读
unknownconf: 当网络预测的“不知道”分数大于此阈值时预测为不知道，否则输出已知分类。
1）与已知类精度关系：当已知类精度越高时，“不知道”在已知类上发生的情况将越少，预测未知类时可以设定更低的unknownconf而不影响已知类性能。
2）与训练集大小关系：训练集越丰富，预测未知类的能力越强
注：可根据需求调节此参数，需要注意的是由于资源问题，在objects365数据集下训练的模型m-obj365.pt仅在小模型下训练了30轮，精度较低，建议采用较高阈值。
其他参数：
1）非极大值抑制：默认类内NMS（非极大值抑制）iou阈值为0.45，参数为iou；同时进行类间NMS，iou阈值为0.75，后续将提供参数接口。
2）不知道的物体类名：可在detect文件中修改，后续将提供接口。             
'''

```
</details>

<details> 
<summary> 视频展示</summary>

1. [demo1](https://b23.tv/MfpEmAm)
2. [demo2](https://www.bilibili.com/video/BV1Nm4y1P7UW/?share_source=copy_web&vd_source=4f63c00122ad06d30c832c5c6f903637)

</details>

## 3. 预训练模型

[s-coco.pt](https://github.com/buxihuo/OW-YOLO/releases/download/0.1/s-coco.pt)<br>
[m-obj365.pt](https://github.com/buxihuo/OW-YOLO/releases/download/0.1/m-obj365.pt)<br>
### coco数据集性能
|Model                       |size<br><sup>(pixels)|mAP<sup>val<br>0.5:0.95 |mAP<sup>val<br>0.5 |
|---                         |---                  |---                     |--- 
|yolov8-n             |640                  |37.3                        |52.6
|OW-yolov8-n          |640                  |37.9 (only known 38)                        |53.7 (only known 53.9)
|OW-yolov8-n-la       |640                  |                        |
```bash
la : label attention

```

## 4. 后续功能
图像分类、实例分割
