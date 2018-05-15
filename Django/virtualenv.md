# VIRTUALENV虚拟环境创建指南

### 前言
virtualenv使用场景:当开发成员负责多个项目的时候，每个项目安装的库又是有很多差距的时候，会使用虚拟环境将每个项目的环境给隔离开来。

### Windows下安装
1.安装virtualenv
```
pip install virtualenv
```
2.创建虚拟环境
注意两个参数：--no-site-packages和-p参数
```
virtualenv --no-site-package venv
```
3.进入/退出env
```
进入　cd env/Scripts/文件夹  在activate命令
退出　deactivate
```


### Ubuntu中安装使用

1.安装virtualenv

```
apt-get install python-virtualenv
```

2.创建包含python3版本的虚拟环境
```
virtualenv -p /usr/bin/python3 env
```

env代表创建的虚拟环境的名称

3.进入/退出env

```
进入 source env/bin/activate

退出　deactivate
```

4.pip使用

查看虚拟环境下安装的所有的包

```
pip list
```

查看虚拟环境重通过pip安装的包

```
pip freeze
```
