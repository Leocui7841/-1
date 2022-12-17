# 机器学习学习笔记
李宏毅教授机器学习(视频地址：https://www.bilibili.com/video/BV1JE411g7XF?p=3&vd_source=0a27b8c0284e7cd3b72bc0c89478f2d7)  
## 第一课：Regression：Case Study  
Regression(回归)，是让我们找到一个函数，使得给定一个input，它可以尽可能地通过这个函数转化成我们想要的output。  
例如我们想要预测一个宝可梦的CP值，也就是我们需要找到一个函数，使得给定一个宝可梦，它能尽可能准确地预测出该宝可梦进化后的CP值。  
首先我们要建立一个model，例如  
y = b + w1 \* xcp，  
y = b + w1 \* xcp + w2 \* (xcp)²,  
……  
接着我们将training data放入我们建立的model中去
