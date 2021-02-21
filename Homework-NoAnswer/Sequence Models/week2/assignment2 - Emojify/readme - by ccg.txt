Author: ccg

本作业缺失数据文件 glove.6B.50d.txt ，下载：

链接：https://pan.baidu.com/s/1XGvG1XGvAEmCHrM-m6goYA 
提取码：qnqp 

下载后放在 data 目录下。

本作业注意：
(1) 1.3 - Implementing Emojifier-V1 中：
word_to_index, index_to_word, word_to_vec_map = read_glove_vecs('data/glove.6B.50d.txt')
可能会报错，需要在 emo_utils.py 的 read_glove_vecs 函数中做以下修改：
#with open(glove_file, 'r') as f:
#modify
with open(glove_file, 'r', encoding = 'utf-8') as f:
修改完之后保存，重启服务重头开始运行即可。