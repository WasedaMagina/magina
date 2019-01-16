---
title: 强化学习超概括总结
date: 2018-04-21 16:20:26
tags: 深度学习总结
categories: 知识总结
mathjax: true
---

### 前言

Udacity深度学习的课程已经学到了最后，本来以为很快就可以做完最后一个项目完成课程。结果强化学习的内容比想象的要多的多，也深的多，花费了很长时间也没完成项目。本文将会概括我近期的学习内容，总结出强化学习的知识框架，以帮助我进一步学习。

### 强化学习要解决什么问题？

一句话总结，强化学习要解决的问题和模糊系统（Fuzzy System）类似，都是复杂环境下的控制问题。

机器和人最大的不同在于人不需要知道知道具体的数值就可以做出动作或者决策，而机器不行。比如说走路，如果要让一个机器走路，实际上就是控制机器人各个关节施加的力，力的大小方向时机搭配合适了，机器人就能成功的走路了，但换一个路面这个搭配可能就不对了，需要重新调整。而人不需要这样，每个人都会走路，然而我们并不知道施加了多少力在关节上，甚至走路主要用到的是哪块肌肉都说不出来，但是人可以走各种各样的路。

有没有一种办法可以让机器人也能用人类的这种方式来做事，就是强化学习要解决的问题。

### 怎么解决？

首先是把转化问题。在走路问题中，评价力的组合是好还是坏事困难的，