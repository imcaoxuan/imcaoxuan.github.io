# apt 镜像


## debian系列
> 在```/etc/apt/auth.conf.d/nexus.local.intranet.conf```文件（若不存在则创建）中添加以下内容
>  ```
>  machine https://mirrors.caoxuan.top:8443/
>  login public
>  password public
>  ```
配置参考 *https://www.caoxuan.top/index.php/archives/80/*

### debian 11
```text
deb https://mirrors.caoxuan.top:8443/repository/apt-proxy-bullseye/ bullseye main
deb https://mirrors.caoxuan.top:8443/repository/apt-proxy-bullseye/ bullseye-updates main
deb https://mirrors.caoxuan.top:8443/repository/apt-proxy-bullseye/ bullseye-backports main

```


## ubuntu系列
直接修改```/etc/apt/source.list```即可

### ubuntu 18.04

```text
deb https://public:public@mirrors.caoxuan.top:8443/repository/apt-proxy-bionic/ bionic main restricted
# deb-src https://public:public@mirrors.caoxuan.top:8443/repository/apt-proxy-bionic/ bionic main restricted

deb https://public:public@mirrors.caoxuan.top:8443/repository/apt-proxy-bionic/ bionic-updates main restricted
# deb-src https://public:public@mirrors.caoxuan.top:8443/repository/apt-proxy-bionic/ bionic-updates main restricted

deb https://public:public@mirrors.caoxuan.top:8443/repository/apt-proxy-bionic/ bionic universe
# deb-src https://public:public@mirrors.caoxuan.top:8443/repository/apt-proxy-bionic/ bionic universe
deb https://public:public@mirrors.caoxuan.top:8443/repository/apt-proxy-bionic/ bionic-updates universe
# deb-src https://public:public@mirrors.caoxuan.top:8443/repository/apt-proxy-bionic/ bionic-updates universe


deb https://public:public@mirrors.caoxuan.top:8443/repository/apt-proxy-bionic/ bionic multiverse
# deb-src https://public:public@mirrors.caoxuan.top:8443/repository/apt-proxy-bionic/ bionic multiverse
deb https://public:public@mirrors.caoxuan.top:8443/repository/apt-proxy-bionic/ bionic-updates multiverse
# deb-src https://public:public@mirrors.caoxuan.top:8443/repository/apt-proxy-bionic/ bionic-updates multiverse

deb https://public:public@mirrors.caoxuan.top:8443/repository/apt-proxy-bionic/ bionic-backports main restricted universe multiverse
# deb-src https://public:public@mirrors.caoxuan.top:8443/repository/apt-proxy-bionic/ bionic-backports main restricted universe multiverse
```

### ubuntu 22.04

```text
deb https://public:public@mirrors.caoxuan.top:8443/repository/apt-proxy-jammy/ jammy main restricted
# deb-src https://public:public@mirrors.caoxuan.top:8443/repository/apt-proxy-jammy/ jammy main restricted

deb https://public:public@mirrors.caoxuan.top:8443/repository/apt-proxy-jammy/ jammy-updates main restricted
# deb-src https://public:public@mirrors.caoxuan.top:8443/repository/apt-proxy-jammy/ jammy-updates main restricted

deb https://public:public@mirrors.caoxuan.top:8443/repository/apt-proxy-jammy/ jammy universe
# deb-src https://public:public@mirrors.caoxuan.top:8443/repository/apt-proxy-jammy/ jammy universe
deb https://public:public@mirrors.caoxuan.top:8443/repository/apt-proxy-jammy/ jammy-updates universe
# deb-src https://public:public@mirrors.caoxuan.top:8443/repository/apt-proxy-jammy/ jammy-updates universe


deb https://public:public@mirrors.caoxuan.top:8443/repository/apt-proxy-jammy/ jammy multiverse
# deb-src https://public:public@mirrors.caoxuan.top:8443/repository/apt-proxy-jammy/ jammy multiverse
deb https://public:public@mirrors.caoxuan.top:8443/repository/apt-proxy-jammy/ jammy-updates multiverse
# deb-src https://public:public@mirrors.caoxuan.top:8443/repository/apt-proxy-jammy/ jammy-updates multiverse

deb https://public:public@mirrors.caoxuan.top:8443/repository/apt-proxy-jammy/ jammy-backports main restricted universe multiverse
# deb-src https://public:public@mirrors.caoxuan.top:8443/repository/apt-proxy-jammy/ jammy-backports main restricted universe multiverse
```


