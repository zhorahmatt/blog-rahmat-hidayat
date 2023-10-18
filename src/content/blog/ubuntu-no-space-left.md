---
title: "Handling 'No Space Left On Device Ubuntu'"
date: 2023-10-17T14:19:44+08:00
draft: false
comments: true
pubDatetime: 2023-10-17T10:11:06.130Z
author: zhorahmatt
description: Here are my personal experience handling this case.
---

I have found this case several times when troubleshooting my app or api that running on our server.

if you find the same problem, here are some action that you may try :

1.  Check how much space you have. You can use `df` or `df -h`
2.  Find large file in your system and delete it
3.  if there are no large file, then you can trace path by path which one that has many files affected your system. you can use `du -h --max-depth=1 /` to analyze which path has bigger size. You can `cd` into the path and delete.
4.  if you are not sure the files you want to delete are affected directly to your system, you may simply copy and rename to different filename and check if your system is running well or not. (this method is not the best practice but it is usefull sometimes when troubleshooting this.)
5.  and also if you have a big size of log on every application you installed, you may back up first if you want to analyze later and delete.

Those are the steps that i usually do when troubleshooting the problem.
