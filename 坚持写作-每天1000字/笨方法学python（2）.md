### 习题1：第一个程序

`print "Hello World!"`

在powershell运行时中，输入`python ex1.py`。

在notepad++运行时，按下设置过的快捷键。

### 习题2：注释和井号

\# 跟在井号背后的都是注释，不会运行

\# this will be ignored in python.



### 习题3：数字和数学计算

`+` 加  `-` 减 `*` 乘 `/ ` 除``%`` 求余 

 `<` 小于 `>` 大于 `<=` 小于或等于 `>=` 大于或等于



### 习题4： 变量和命名

`cars = 100`

`drivers = 30`

` cars_not_driven = cars - drivers`

### 习题5：更多的变量

**格式化字符**

`my_name = 'Zed A. Shaw'`

`my_htight = 35`

`print "Let's talk about %s." %my_name`

`print "He's %d inches tall." %my_height`

> %s 代表字符；%d 代表整数；%r 打印所有

### 习题6：字符串和文本

`binary = 'binary'`

`x = "There are %d types of people." % 10`

`y = "Those who know %s and those %s."%(binary, do_not)`

\# 注释：多个变量间用逗号`,`隔开

注意双引号与单引号互相嵌套的情形。

### 习题7：更多打印

` print "Tis fleece was white as %s." % 'snow' `

(格式化字符里的字符串)

`+`加号可以连接字符：

> "c" + "h" +"i" + "n"+ "a"

### 习题8：打印，打印

> %r 可以打印所有

`formatter = '%r %r %r %r'`

`print formatter %(1,2,3,4)`

`print formatter %("one","two","three","four")`

### 习题9：打印，打印，打印，打印

`print """`

`There's something going on here.`
`With the three double-quotes.`
`We'll be able to type as much as we like.`
`Even 4 lines if we want, or 5, or 6.`
`"""`

`months = "Jan\nFeb\nMar\nApr\nMay\nJun\nJul\nAug"`

> 三引号，里面的代码可以换行

或者用`\n`换行

### 习题10： 那是什么（转义符）

**转义符** `\`

`\t`是制表符

`\n`是换行符

`\\`显示斜杠

### 习题11：提问

**输入**

`print "How old are you?",`
`age = raw_input()`

> print后面有个逗号`,`，防止输出后直接跳到下一行

### 习题12：提示别人

`age = raw_input("How old are you? ")`

> raw_input 提示别人输入

**帮助文档**

用`pydoc`查看文档，`python -m pydoc raw_input`

在python的编译环境下，用help()查看

### 习题13：参数、解包、变量

```python
from sys import argv

script, first, second, third = argv

print "The script is called:", script
print "Your first variable is:", first
print "Your second variable is:", second
print "Your third variable is:", third
```

用下面的方法运行你的程序：（必须传递三个参数）

`python ex13.py first 2nd 3rd` (在powershell里输入)

first、second、third就是三个变量。

> - 记住“模块”（modules）这个单词，多读几遍。
> - raw_input和argv一起使用，让你的脚本从用户手上得到更多的输入

### 习题14：提示和传递

```python
from sys import argv

script, user_name = argv
prompt = '> '

print "Hi %s, I'm the %s script." % (user_name, script)
print "I'd like to ask you a few questions."
print "Do you like me %s?" % user_name
likes = raw_input(prompt)

print "Where do you live %s?" % user_name
lives = raw_input(prompt)

print "What kind of computer do you have?"
computer = raw_input(prompt)

print """
Alright, so you said %r about liking me.
You live in %r.  Not sure where that is.
And you have a %r computer.  Nice.
""" % (likes, lives, computer)
```

### 习题15：读取文件

两个文件：`ex15.py`和`ex15_sample.txt`

```python
from sys import argv

script, filename = argv

txt = open(filename)

print "Here's your file %r:" % filename
print txt.read()

print "Type the filename again:"
file_again = raw_input("> ")

txt_again = open(file_again)

print txt_again.read()
```

`txt= open(readme.txt)` 和`txt.read()`

> 不需要看那些双下划线__的命令，那些都是垃圾。

最后执行以下`close()`

### 习题16：读写文件

- close——关闭文件
- read——读取文件内容
- readline——读取文本文件中的一行
- truncate——清空文件
- write(stuff)——将stuff写入文件

```python
target = open(readme.txt, 'w')
line1 = raw_input("line 1: ")
target.write(line1)
target.close()
```

> 一个小技巧，让你的文件先运行一小部分，比如先运行1—8行

### 习题17：更多文件操作

exists 检查文件是否存在，在，则返回True。

### 习题18：命名、变量、代码、函数

```python
def print_two(*args):
    arg1, arg2 = args
    print "arg1: %r, arg2: %r" % (arg1, arg2)
def print_two_again(arg1, arg2):
    print "arg1: %r, arg2: %r" % (arg1, arg2)
print_two("Zed","Shaw")
print_two_again("Zed","Shaw")  
```

### 习题19：函数和变量

同上

### 习题20：函数和文件

```python
def print_all(f):
    print f.read()
current_file = open (readme.txt)
print_all(current_file)
```

### 习题21：函数可以返回东西

```python
def add(a, b):
    print "ADDING %d + %d" % (a, b)
    return a + b
```

### 习题22：到现在你学到了哪些东西？



把你所学到的全部列出来。



### 习题23：读代码



使用你目前学到的知识，看是否能读懂一些代码。



不懂的，记下来。



### 习题24：更多练习

### 习题25： 更多更多的练习



### 习题26：恭喜你，现在可以考试了

修改别人的糟糕的代码。
