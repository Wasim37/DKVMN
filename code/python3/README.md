MXNet�ٷ��ĵ����İ�̳�(1)���̳̣�Tutorials��
https://blog.csdn.net/qq_36165459/article/details/78394199

MXNet��Model API
https://blog.csdn.net/qq_25491201/article/details/51386435


������ʵ���԰�һ��symbol�����Ǿ��ж�������ĺ��������������µķ���������Щ������
net.list_arguments()

����ÿ�����ţ����ǿ���ѯ�������루���߲������������
arg_name = c.list_arguments() # get the names of the inputs 
out_name = c.list_outputs() # get the names of the outputs

bind��ͨ���ڴ����Ϊ��������
init_params ����ʼ������
init_optimizer����ʼ���Ż�����Ĭ����sgd
metric.create��������ָ�����ƴ�������ָ��
forward ��ǰ�����
update_metric�������һ��ǰ��������������������ۼ���������
backward ���������
update �����ݰ�װ���Ż��������ǰ��ǰ����������м�����ݶȸ��²���