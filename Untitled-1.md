# Matlab学习笔记
- [Matlab学习笔记](#matlab学习笔记)
  - [Matlab常用关键词](#matlab常用关键词)
  - [Matlab常用语法](#matlab常用语法)
  - [Matlab预宣告](#matlab预宣告)
  - [小技巧](#小技巧)
  - [自定义函数](#自定义函数)
  - [cell array](#cell-array)

## Matlab常用关键词
1. rem(a,2) 取余
2. disp('')  显示
3. prod(a:n) 阶乘
4. 1e100  科学计数法
5. `tic toc` 计算运行时间
6. mean(a)平均数
7. edit(which('__.m'))打开函数
8. zero[10]10个0  zero[10 10] 10*10矩阵
9. whos 可以查看变量类型和数量
## Matlab常用语法
- **if语句**
```matlab
if  rem(a,2)==0
    condition1
else
    condition2
end
```
- **switch语句**
```matlab
switch number
case -1
    disp();
case 0
    disp();
otherwise
    disp();
end
```
- **while语句**
```matlab
while prod(1:n)<1e100
    n=n+1;
end
```
- **for语句**
```matlab
for variable=start:increment:end
    commands
end
```
P.S. ***increment可以不写,不写默认为1***
- **break指令**
跳出循环.
## Matlab预宣告
可以加快运行速度
方法:
    提前为矩阵划分空间.
## 小技巧
1. `clc` 清屏
2. `clear all`to remove previous variables
3. `close all`to close all figures
4. `semicolon`不显示执行结果
5. `...`换行
6. CTRL C 停止运行
7. 函数([1 1 2])可一次算出多组数值 (P.S.用点乘法)
8.  str (str=='a')='z' 将a替换为z.
## 自定义函数
**语法:**
`function y=mean(x)`
|function|y|mean(x)|
 arr
|keyword|output|input|- 
## cell array
using {}
A(1,1)={[1 2 3;4 5 6;7 8 9]}
A{1,1}=[1 2 3;4 5 6;7 8 9]
a=magic(3)创建一个任意数组
num2cell将每一个元素变成矩阵
mat2cell(a,[1,1,1],3)a矩阵，3行，3列和一
