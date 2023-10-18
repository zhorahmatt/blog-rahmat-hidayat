---
title: "Allow Spesific IP and Port Ubuntu"
date: 2023-10-18
draft: false
comments: true
pubDatetime: 2023-10-18
author: zhorahmatt
description: ""
---

Here is how to allow spesific IP & Port via UFW

Say if we want to allow 121.111.231.234 with port 3310 on TCP, you can type :
`sudo ufw allow from 121.111.231.234 proto tcp to any port 3310`

you can view the result :
![Slow Build Time Gitlab Ci With Yarn](/assets/ufw.png)

To delete the rules with :
`sudo ufw delete allow from 10.0.0.46 proto tcp to any port 3310`
