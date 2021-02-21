Author: ccg

本作业注意：
作业2 Convolution model - Application - v1 中，按照题目给定的参数最后的训练效果
可能会很差，估计是因为tensorflow的版本不同问题。
可进行如下的参数设定，最后训练效果很好(题目要求8*8，改成6*6)：
	# MAXPOOL: window 8x8, sride 8, padding 'SAME'
	P1 = tf.nn.max_pool(A1, ksize = [1,6,6,1], strides = [1,6,6,1], padding = 'SAME')
	(测试版本：tensorflow-1.13.0  python-3.6.8)
与此同时，后面步骤得到的期望输出都和题目要求也会不同。