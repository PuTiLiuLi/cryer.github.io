---
layout: post
title: win10安装pytorch教程
description: 因为官方pytorch不支持windows版本，所以这里给出其他的方法来安装
---


# 前提条件
首先你需要是windows10系统，专业版家庭版都可以
然后你已经安装了Anaconda 3.5/3.6
最后你已经配置好了cuda8.0和cudnn

#开始安装
安装蒲嘉宸的安装包，注意对应的python版本和cuda版本，我这里给出python3.5和cuda8.0的安装包百度云分享
		
		[链接](https://pan.baidu.com/s/1c2ppDFM) 
		密码：bq77

然后打开命令提示符，依次输入：

		conda create -n mypytorch python = 3.5

		activate mypytorch

		conda install --offline D:\pytorch-0.1.12-py35_0.1.12cu80.tar.bz2

		conda install nb_conda

其中，第一步是建立py3.5的虚拟环境，名字叫mypytorch，这个可以自定义，然后激活环境，离线安装我给出的安装包，地址根据实际地址
最后在线安装nb_conda。

# 测试

测试只需要打开jupyter notebook 输入

		import torch

如果没有报错，代表安装成功，并且可以使用cuda加速。

感谢蒲嘉宸大佬=-=



