Author: ccg

本作业注意：
(1) 5 - Model with different optimization algorithms 中做以下修改(3处)：
#plot_decision_boundary(lambda x: predict_dec(parameters, x.T), train_X, train_Y)
#modify
plot_decision_boundary(lambda x: predict_dec(parameters, x.T), train_X, train_Y[0, :])