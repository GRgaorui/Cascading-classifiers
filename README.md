# OpenCV-Cascade-Classifier
使用OpenCV的级联分类器识别中国象棋棋子

Dataset_Red_Black文件夹保存了采集的棋子图片，是经过灰度化及中值滤波后的图片，红色棋子和黑色棋子图片分开保存，每种颜色7类棋子，每类棋子经筛选后保留200张各种角度的图片。

model_save文件夹保存了使用上述数据集训练好的级联分类器模型，包括红色棋子分类模型Red_Chess.yml和黑色棋子分类模型Black_Chess.yml，该模型可在recognize.py中直接使用。

TestPicture文件夹保留了4张用于测试的图片，检测模型分类的准确率。

##### getDataSet.py:

运行该程序，手动转动棋子，采集棋子各角度图片用于训练模型。

##### train.py:

使用级联分类器训练分类模型。

##### recognize.py:

测试模型效果，TestPicture文件夹中有几张测试图片，也可直接处理摄像头实时画面。
