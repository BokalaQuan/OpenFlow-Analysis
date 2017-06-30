# 深度解析OpenFlow

## 第一部分 OpenFlow概述

### 为什么学习OpenFlow？

* 实践 **SDN** 的首选
* 主流南向接口
* **P4** 的 **PISA** 架构的前身

### OpenFlow起源

* **Ethane** 项目是 **OpenFlow** 的前身
* 2008年的 **OpenFlow** 论文
* **OpenFlow** 最初用于网络实验


### OpenFlow最初的定义( *The Mckeown Group* )

> OpenFlow is an open standard that enables researchers to run experimental protocols in the campus networks we use every day.
>
> OpenFlow is added as a feature to commercial Ethernet switches, routers and wireless access points, and provides a stanardized hook to allow researchers to run experiments, without requiring vendors to expose the internal workings of their network devices.

### OpenFlow 是什么？

**开放的南向接口 + 通用的转发抽象模型 + 网络X86指令集**

1. 开放的南向接口

![1](/home/bokala/Documents/OpenFlow-Analysis/1.png)

2. 通用转发抽象模型

![2](/home/bokala/Documents/OpenFlow-Analysis/2.png)

![3](/home/bokala/Documents/OpenFlow-Analysis/3.png)

### OpenFlow发展历史

| Version | DaTE     | STATIStics                | matches | actions | instructions |
| ------- | -------- | :------------------------ | :-----: | :-----: | :----------: |
| OF 1.0  | Dec 2009 | Per table/flow/port/queue |   12/   |   13/   |      1       |
| OF 1.1  | Feb 2011 | Group/Action bucket       |   15/   |   32/   |      0       |
| OF 1.2  | Dec 2011 | ...                       |   36/   |   51/   |      5       |
| OF 1.3  | Jun 2012 | Per flow meter            |   40/   |   58/   |      6       |
| OF 1.4  | Oct 2013 | Optical port properties   |   41/   |   59/   |      6       |

![5](/home/bokala/Documents/OpenFlow-Analysis/5.png)

## 第二部分 OpenFlow通用抽象

### OpenFlow中的术语

![6](/home/bokala/Documents/OpenFlow-Analysis/6.png)

![7](/home/bokala/Documents/OpenFlow-Analysis/7.png)

### OpenFlow Switch-通用转发抽象模型

![8](/home/bokala/Documents/OpenFlow-Analysis/8.png)

![9](/home/bokala/Documents/OpenFlow-Analysis/9.png)

### Flow Table处理流程一览

![10](/home/bokala/Documents/OpenFlow-Analysis/10.png)

### 多级流表处理一览

![11](/home/bokala/Documents/OpenFlow-Analysis/11.png)

### Flow Table-流表子模型

![12](/home/bokala/Documents/OpenFlow-Analysis/12.png)

![13](/home/bokala/Documents/OpenFlow-Analysis/13.png)

### Flow Entry-流表项

![14](/home/bokala/Documents/OpenFlow-Analysis/14.png)

### Match Fields-流表项匹配域

![15](/home/bokala/Documents/OpenFlow-Analysis/15.png)

### OXM的TLV匹配域描述

![16](/home/bokala/Documents/OpenFlow-Analysis/16.png)

### OXM TLV的基本结构

![17](/home/bokala/Documents/OpenFlow-Analysis/17.png)







































