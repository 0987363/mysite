+++
title = "在goji中跨域"
description = ""
tags = [
    "golang",
    "cors",
    "goji",
    "development",
]
date = "2016-08-02"
categories = [
    "Golang",
    "Goji",
    "Development",
]
+++

## 最近用goji框架，当前端是web的时候，跨域请求:

```golang
import "github.com/rs/cors"

c := cors.New(cors.Options{
    AllowedOrigins: []string{"http://www.github.com", "http://xxx.com"},
    AllowedMethods: []string{"POST", "GET", "UPDATE", "DELETE", "PUT"},
    AllowedHeaders: []string{"X-XXX-Authentication", "Content-Type", "Origin", "Accept-Language", "Accept"},
    ExposedHeaders: []string{"X-XXX-Authentication"},
})  
v1Mux.Use(c.Handler)

```

