---
title: docker
date: 2019-04-30 10:09:34
category:
- notes
tags:
- notes
- docker
---

## ARG

### Dockerfile

在Dockerfile中
```dockerfile
ARG <name>[=<default value>]
```
使用时形如${user:-some_user}，意思是如果变量不存在，默认值是-some_user。不用大括号应该也可以。

在命令行通过--build-arg传入

```
$ docker build --build-arg key=value .
```

在ARG之前使用变量会有warning，只有ARG后的变量引用才会读取命令行里的参数。

### docker-compose

```yaml
build:
  context: .
  args:
  	- key=value
```

发现build可以直接是值，也可以是map。