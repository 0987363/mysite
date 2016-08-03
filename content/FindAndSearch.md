+++
title = "搜索文件内容，然后去重复，复制"
description = ""
tags = [
    "shell",
    "xargs",
    "awk",
    "cp",
]
date = "2016-08-02"
categories = [
    "Linux",
    "Shell",
]

+++

```
find . -name "*JULIA*" | awk -F "/" '{print $2}' | uniq | xargs -i cp -rf {} ~/base/temp
```
