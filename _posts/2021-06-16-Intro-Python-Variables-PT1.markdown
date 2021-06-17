---
layout: post
title:  "Introduction to Python Variables Part 1"
date:   2021-06-16 17:47:45 -0400
#last_modified_at:
lang: zh-Hans
categories: python
tags: 教程
---

我前几年上了一个数据分析可视化bootcamp。自从开始做Salesforce就没有怎么去学习Python了。走在自我提升道路上决定从复习开始。

<strong>环境:</strong>
1. 安装环境管理器：Anaconda
2. 安装Python，创建环境：Terminal输入 ‘conda create -n PythonData python=3.6 anaconda' （PythonData是环境的名字。当时上bootcamp，python stable release是3.6）
3. 从Terminal进入环境输入：‘source activate PythonData’
4. 结束环境Terminal输入： ‘source deactivate’
5. 如果不想安装什么，可以用在线IDE：Repl.it

Activity ‘Input Data Variables':

<strong>Instructions</strong>
1. Collect the user's input for the prompt "What is your name?" 收集用户输入的名字。
2. Collect the user's input for the prompt "How old are you?" and converts the string to an integer. 收集用户输入的年龄并将字符串转换为整数。
3. Collect the user's input for the prompt "Is input true?" and converts it to a Boolean. 收集用户回答并将转换为布尔变量。
4. Create three print statements that to respond with the output. 用print() 方法用于打印输出


<pre><code>
  # Collect the user's input for the prompt "What is your name?" 收集用户输入的名字。
  name = input("What is your name?")
  # Collect the user's input for the prompt "How old are you?" and converts the string to an integer. 收集用户输入的年龄并将字符串转换为整数。
  age = int(input("How old are you?"))
  # input() 函数接受一个标准输入数据，返回为 string 类型，所以用 ‘int’ 来转换为整数。
  # Collect the user's input for the prompt "Is input true?" and converts it to a Boolean. 收集用户回答并将转换为布尔变量。
  trueOrFalse = bool(input("Is the input true?"))
  # 任何input会显示True。只有null input才会显示False
  # Create three print statements that to respond with the output. 用print() 方法用于打印输出
  print("My name is " + str(name))
  print("I will be " + str(age + 1) + " next year.")
  print("The input was converted to " + str(trueOrFalse))
</code></pre>

![Replit Screenshot](/image/ReplitPost61621.png)




