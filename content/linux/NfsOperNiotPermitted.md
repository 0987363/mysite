+++
title = "nfs远程挂载报错：Operation not permitted"
description = ""
tags = [
    "nfs",
    "linux",
]
date = "2016-08-02"
categories = [
    "Linux",
    "Nfs",
]

+++

远程挂载nfs的时候报错，提示Operation not permitted，加入`-o resvport`即可.
```
sudo mount_nfs -o resvport 192.168.0.100:/mnt/raid1/media /Volumes/media
```
