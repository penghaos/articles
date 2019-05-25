可复制到typora中查看流程图：
``` 
#（代码用```框起来，即数字1左边的`）
# 语言选择flow语言
# 这个流程图对应 Learn python3 by the hard way 中的ex35.py的流程

st=>start: 开始
e=>end: 结束
op1=>operation: 进入bear_room()
op2=>operation: dead()
op3=>operation: 进入cthulhu_room()
op4=>operation: dead()
op5=>operation: 操作5
op6=>operation: I can't understand
op7=>operation: 进入gold room
op8=>operation: 操作8
op9=>operation: succeed
sub1=>subroutine: 下面的模块

cond1=>condition: 左边?
cond2=>condition: 右边？
cond3=>condition: take money?
cond4=>condition: taunt bear?
cond5=>condition: open door?
cond6=>condition: taunt bear？
cond7=>condition: "0"or"in"?
cond8=>condition: <50？
cond10=>condition: flee？
cond11=>condition: eat head?

st->cond1
cond1->cond2
cond1->op1
cond1(yes)->op1
cond1(no)->cond2
cond2(no)->op2
cond2(yes)->sub1

op1->cond3
cond3(yes)->op4
cond3(no)->cond4
cond4->op5
cond4(yes)->cond5
cond4(no)->op6
op6(right)->op1
cond5(yes)->op7
cond5(no)->cond6
cond6(yes)->op2
cond6(no)->cond5
op7->cond7
cond7(no)->op2
cond7(yes)->cond8
cond8(no)->op2
cond8(yes)->op9

op9->e
```
![image.png](https://upload-images.jianshu.io/upload_images/197369-fdfb9ab51074501c.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


```
sub1=>subroutine: 下面的模块,这是子程序
op1=>operation: 进入 cluthlu房间
op2=>operation: dead
op3=>operation: 回到最开始
cond1=>condition: flee？
cond2=>condition: eat your head?

sub1->op1->cond1
cond1(yes)->op3
cond1(no)->cond2
cond2(yes)->op2
cond2(no)->op1
```
![image.png](https://upload-images.jianshu.io/upload_images/197369-b8914f0277bbfc09.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

``` 
io1=>inputoutput: 这是输入或输出
op1=>operation: 这是操作符
io1->op1
```
![image.png](https://upload-images.jianshu.io/upload_images/197369-1ca67e73a656a20d.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


参考教程：

[mardown Flowchart基础教程]: (https://blog.csdn.net/KimBing/article/details/52934959 )
[Markdown Flowchart参考教程]: (https://blog.csdn.net/subson/article/details/75126945 ）
