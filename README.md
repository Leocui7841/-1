# 机器学习学习笔记
李宏毅教授机器学习(视频地址：https://www.bilibili.com/video/BV1JE411g7XF?p=3&vd_source=0a27b8c0284e7cd3b72bc0c89478f2d7)  
## 第一课：Regression：Case Study  
Regression(回归)，是让我们找到一个函数，使得给定一个input，它可以尽可能地通过这个函数转化成我们想要的output。  
例如我们想要预测一个宝可梦的CP值，也就是我们需要找到一个函数，使得给定一个宝可梦，它能尽可能准确地预测出该宝可梦进化后的CP值。  
首先我们要建立一个model，例如  
y = b + w1 \* xcp，  
y = b + w1 \* xcp + w2 \* (xcp)²,  
……  
我们通过training data构建了这个model，接着我们将testing data放入我们建立的model中去计算我们预测的cp值与实际的cp值之间的偏差，以此用来代表我们的model的好坏程度。  
我们发现，在一定程度上我们的model表达式越复杂，它的预测效果就越好，但是当表达式过于复杂的时候，我们的预测效果反而会变得很糟糕，这种现象我们称之为**Overfitting**，所以我们的model并不是越复杂就越好的，构建一个合适的model就成了一个非常关键的问题。
