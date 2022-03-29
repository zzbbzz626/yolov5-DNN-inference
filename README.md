# yolov5-DNN-inference

对YOLOV5官网网站推荐的DNN(C++版)推理代码的学习心得，源代码地址为：https://github.com/doleron/yolov5-opencv-cpp-python

OpenCV version >= 4.5

![Image text](https://github.com/zzbbzz626/images/blob/main/1648533010(1).jpg)

YOLO检测头的大小可以通过上图计算过程计算

![Image text](https://github.com/zzbbzz626/images/blob/main/1648533043(1).jpg)

当采用单分类时检测头预测厚度为[x,y,w,h,conf,cls] cls=class number，因此图中的厚度为6

在更改推理模型为自己训练的不同版本的YOLOV5推理出的onnx文件时，只需要更改程序的78、79行中的dimensions=自己训练模型的厚度，row=3x((img/8)^2+(img/16)^2+(img/32)^2)即可。
