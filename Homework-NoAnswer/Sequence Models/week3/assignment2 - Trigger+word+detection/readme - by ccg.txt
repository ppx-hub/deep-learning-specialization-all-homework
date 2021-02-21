Author: ccg

本作业缺失数据文件 X.npy ，下载
链接：https://pan.baidu.com/s/1kJHnSDDyizX5t5gVltP9sw 
提取码：68su 
下载后放在 XY_train 目录下;

缺失数据文件 X_dev.npy ，下载
链接：https://pan.baidu.com/s/1c-eHd_qgaXkUNFIBzO6TXg 
提取码：4tun 
下载后放在 XY_dev 目录下。


本作业注意：
(1) 2.2 - Fit the model 中进行

model.fit(X, Y, batch_size = 5, epochs=1)

后，效果可能会变得很差，可能是keras版本变更导致，
可以注释掉此行，直接利用预加载好的模型进行预测。
