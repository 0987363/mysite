+++
title = "通过mgo用正则表达式搜索mongodb"
description = ""
tags = [
    "mgo",
    "mongo",
    "golang",
    "development",
]
date = "2016-08-02"
categories = [
    "Mongodb",
    "Golang",
    "Development",
]

+++

```
c.Find(bson.M{"abc": &bson.RegEx{Pattern: "abc", Options: "i"}})
```

