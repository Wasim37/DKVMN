MXNet官方文档中文版教程(1)：教程（Tutorials）
https://blog.csdn.net/qq_36165459/article/details/78394199

MXNet的Model API
https://blog.csdn.net/qq_25491201/article/details/51386435


我们其实可以把一个symbol看做是具有多个参数的函数，可以用以下的方法遍历这些参数：
net.list_arguments()

对于每个符号，我们可以询问其输入（或者参数）和输出。
arg_name = c.list_arguments() # get the names of the inputs 
out_name = c.list_outputs() # get the names of the outputs

bind：通过内存分配为计算搭建环境
init_params ：初始化参数
init_optimizer：初始化优化器，默认是sgd
metric.create：从输入指标名称创建评估指标
forward ：前向计算
update_metric：对最后一次前向计算的输出进行评估和累加评估度量
backward ：后向计算
update ：根据安装的优化程序和先前的前向后向批次中计算的梯度更新参数