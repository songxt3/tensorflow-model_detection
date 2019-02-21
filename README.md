# tensorflow-model_detection
使用tensorflow-model_detection模块训练自己的模型用来进行物体检测
## 项目介绍
1. 使用[labelImg](https://github.com/tzutalin/labelImg)给预先找好的花朵图片标注标签，生成xml文件  
2. 使用[datitran](https://github.com/datitran/raccoon_dataset)将xml文件转化为record文件  
3. 选择一个[coco数据集](https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/detection_model_zoo.md)预训练的模型，修改配置文件  
4. 使用tensorflow/object\_detection/legacy/train.py进行模型训练  
5. 使用tensorflow/object\_detection/export\_inference\_graph.py生成自己的模型  

## 文件说明
**data**：存放训练数据  
**src**：存放训练和预测代码