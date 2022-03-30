# yolov5-DNN-inference

For reference, please give me a star！ Please Please!

The learning experience of the DNN (C++ version) reasoning code recommended by the YOLOV5 official website website, the source code address is：https://github.com/doleron/yolov5-opencv-cpp-python

OpenCV version >= 4.5

![Image text](https://github.com/zzbbzz626/images/blob/main/1648533010(1).jpg)

The size of the YOLO detection head can be calculated through the calculation process shown in the figure above.

![Image text](https://github.com/zzbbzz626/images/blob/main/1648533043(1).jpg)

The detection head of the inspection head is[x,y,w,h,conf,cls] cls=class number。When single classification is used, cls=1, so the thickness in the figure is 6

When changing the onnx file inferred by the inference model for different versions of YOLOV5 trained by yourself, you only need to change the dimensions in lines 78 and 79 of the program = the thickness of your own training model，row=3x((img/8)^2+(img/16)^2+(img/32)^2)。
