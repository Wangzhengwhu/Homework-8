# Homework-8  
##摘要
主要解决书上的3.4，3.5的题目，主要分析了非简谐振动的周期与非简谐力之间的的具体关系，主有Euler methond,Euler-cromer methond,Runge-Kutta methond，本文主要采用Euler-cromer methond,并对不同的计算方法进行对比。
##正文
###周期的解析式
非简谐运动的运动微分方程：  
dx^2/d^2t = - kx^a  
运动过程中最大的位移  
xm  
上式的解析式即运动解为  
![解析式](https://github.com/Wangzhengwhu/Homework-8/blob/master/%E8%A7%A3%E6%9E%90%E5%BC%8F.png)  
当a=1时，T = 2pi sqrt((a+1)/k) ,若a不为1时，周期T与xm最大位移相关。  

###不同计算方法的比较
我们以二阶常微分方程为例  
dx^2/d^2t = -x  
x(0) = 1  
x'(0)= 0  
可以得到解析解为  
x(t) = cos(t)  
接下来利用Euler methond，Euler-cromer methond,Runge-Kutta方法分别计算  
[程序](https://github.com/Wangzhengwhu/Homework-8/blob/master/1.py)  
![计算结果对比图](https://github.com/Wangzhengwhu/Homework-8/blob/master/1.png)  

###非简谐运动
dx^2/d^2t = - kx^a  
利用四阶R—K算法计算其数值解，在k = 1 , a = 1,2,3,4时的计算结果  
[程序](https://github.com/Wangzhengwhu/Homework-8/blob/master/5.py)  
![计算结果对比图](https://github.com/Wangzhengwhu/Homework-8/blob/master/2.png)  

