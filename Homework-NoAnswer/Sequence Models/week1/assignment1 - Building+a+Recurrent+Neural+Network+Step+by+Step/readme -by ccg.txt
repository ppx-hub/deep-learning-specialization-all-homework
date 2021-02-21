Author: ccg

本作业注意：
(1) 3.3 Backward pass through the LSTM RNN 中 lstm_backward 得到的输出：

gradients["dx"][1][2] = [-0.00173313  0.08287442 -0.30545663 -0.43281115]
gradients["dx"].shape = (3, 10, 4)
gradients["da0"][2][3] = -0.09591150195400468
gradients["da0"].shape = (5, 10)
gradients["dWf"][3][1] = -0.06981985612744009
gradients["dWf"].shape = (5, 8)
gradients["dWi"][1][2] = 0.10237182024854771
gradients["dWi"].shape = (5, 8)
gradients["dWc"][3][1] = -0.062498379492745226
gradients["dWc"].shape = (5, 8)
gradients["dWo"][1][2] = 0.04843891314443012
gradients["dWo"].shape = (5, 8)
gradients["dbf"][4] = [-0.0565788]
gradients["dbf"].shape = (5, 1)
gradients["dbi"][4] = [-0.15399065]
gradients["dbi"].shape = (5, 1)
gradients["dbc"][4] = [-0.29691142]
gradients["dbc"].shape = (5, 1)
gradients["dbo"][4] = [-0.29798344]
gradients["dbo"].shape = (5, 1)

与期望的输出：

gradients["dx"][1][2] = [-0.00173313 0.08287442 -0.30545663 -0.43281115]
gradients["dx"].shape = (3, 10, 4)
gradients["da0"][2][3] = -0.095911501954
gradients["da0"].shape = (5, 10)
gradients["dWf"][3][1] = -0.0698198561274
gradients["dWf"].shape = (5, 8)
gradients["dWi"][1][2] = 0.102371820249
gradients["dWi"].shape = (5, 8)
gradients["dWc"][3][1] = -0.0624983794927
gradients["dWc"].shape = (5, 8)
gradients["dWo"][1][2] = 0.0484389131444
gradients["dWo"].shape = (5, 8)
gradients["dbf"][4] = [-0.0565788]
gradients["dbf"].shape = (5, 1)
gradients["dbi"][4] = [-0.06997391]
gradients["dbi"].shape = (5, 1)
gradients["dbc"][4] = [-0.27441821]
gradients["dbc"].shape = (5, 1)
gradients["dbo"][4] = [ 0.16532821]
gradients["dbo"].shape = (5, 1)

后几个数值可能会不同，原因未知。（可能是答案写错了？）
