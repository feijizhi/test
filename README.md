# test
This is a description
# 1，中国国旗

参考数据:

```python
t.seth(0)#调整星星角度
t.rt(72)
draw_star(-400,320,228)#星星坐标+线长

t.seth(0)
t.rt(162)
draw_star(-160,40,75)

t.seth(0)
t.rt(162)
draw_star(-160,320,75)

t.seth(0)
t.rt(72)
draw_star(-120,160,75)

t.seth(0)
t.rt(252)
draw_star(-120,200,75)
```





# 2，表情包+美队盾牌



# 3，正反九九表

用双循环法

# 4，直方图

### 1，描线法直方图

### 2，填充法直方图

提供数据：长+宽

```python
ls=[[69,15],[292,10],[33,8],[131,10],[61,5],[254,10],[100,15],[80,25]]

x0=-200 y0=-100 #坐标轴原点坐标
```

步骤：

1.初始化
2.定义模块
3.画坐标轴
4.画直方图

# 5，四种排序（升序）

三种选择排序+冒泡排序
1.原始选择排序
2.改进型选择排序
3.最优性选择排序

数据：

```python
ls=[12,40,10,9,8,-1,21,-6]
```



# 6，美国国旗+奥运五环

### 一，美国国旗

```python
def draw_flag():#画旗面 长1200，宽650
    move(-600,325)
    t.pencolor('black')
    for i in range(2):
        t.fd(1200)
        t.rt(90)
        t.fd(650)
        t.rt(90)
......        

```



### 二，奥运五环

```python
t1=t.Turtle()#申请两只画笔
t2=t.Turtle()

t1.pensize(20)
t2.pensize(20)

t1.pencolor('red')#画红色圈
move(220,-100)
t1.circle(100)

t2.pencolor('green')#画绿色圈
move_(110,-200)
t2.circle(100) 

t1.pencolor('black')#画黑色圈
move(0,-100)
t1.circle(100)

t2.pencolor('yellow')#画黄色圈
move_(-110,-200)
t2.circle(100) 

t1.pencolor('blue')#画蓝色圈
move(-220,-100)
t1.circle(100)
```



# 7，孪生素数

思路如下：

1.设定要求的范围
2.将其中的所有素数装入一个列表
3.将素数列表中相邻的两个素数单独拿出来进行判断，若满足孪生素数的关系，就将这一对装入一个新的列表

需要注意：

```python
        if(i%j==0):
            break
    else:         #这里的if不能与else同辈，因为j取不同值时，同一个i可能多次满足，则i会被多次存入列表
        list.append(i)

```

因为0和1既不是素数也不是合数，所以所输入的范围最小值要大于等于1
