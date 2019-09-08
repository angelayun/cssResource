* counter-reset 相当于给计数器起个名字，如果可能顺便告诉下从哪个数字开始计数，默认是0
* 如果是多个计数的话，直接空格分隔
* counter-increment 表示计数器递增
* 普照源（counter-reset）唯一，每普照（counter-increment）一次，普照源增加一次计数值，只要有counter-increment对应的计数器的值才会变化，counter()只是输出而已
* 变化的值不一定是1，变化的值还可以是负数
```
counter-increment:counter 2;
```
* **显示content计数值的那个dom元素在文档流中的位置一定要以counter-increment元素的后面，否则是没有计数效果的**
* content内容生成语法是可以混全一起使用的，如果我们希望伪元素中同时显示图片和文字排列效果，其实只需要一个伪元素即可