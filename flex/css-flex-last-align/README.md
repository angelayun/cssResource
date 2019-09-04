[让CSS flex布局最后一行列表左对齐的N种方法](https://www.zhangxinxu.com/wordpress/2019/08/css-flex-last-align/)


1.假设是1行4个的话，那就需要把每1行前3个的marginRight进行calc计算
2.计算最后1行最后1个元素距离右侧的宽度，但是需要假设一行5个的话，那需要考虑最后一行只有2个、只有3个、只有4个的情况
3.最后一个元素margin:auto即可
4.在父容器上增加after伪元素让它flex为1或auto
5.使用足够的空白标签进行填充占位，具体的占位数量是由最多列数的个数决定的
6.使用grid布局
