# pypi 镜像

## 简介
PyPI(Python Package Index)是Python编程语言的软件存储库。开发者可以通过PyPI查找和安装由Python社区开发和共享的软件，也可以将自己开发的库上传至PyPI。

## 配置

a. 在```~/.pip/pip.conf```文件中添加或修改:
```shell
[global]
index = https://public:public@mirrors.caoxuan.top:8443/repository/pypi-proxy/pypi
index-url = https://public:public@mirrors.caoxuan.top:8443/repository/pypi-proxy/simple
```
b. 设为默认
升级 pip 到最新的版本 (>=10.0.0) 后进行配置：
```shell
python -m pip install --upgrade pip
pip config set global.index-url https://public:public@mirrors.caoxuan.top:8443/repository/pypi-proxy/simple
```

