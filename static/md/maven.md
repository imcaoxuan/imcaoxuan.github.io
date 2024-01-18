# maven 镜像

## 简介

CX Maven中央仓库为CX提供的公共代理仓库，帮助研发人员提高研发生产效率，使用CX Maven中央仓库作为下载源，速度更快更稳定。

## 配置方法

### maven 配置

打开 maven 的配置文件(windows机器一般在maven安装目录的conf/settings.xml)，在```<mirrors></mirrors>```标签中添加 mirror
子节点:

```xml

<mirror>
    <id>cxmaven</id>
    <mirrorOf>*</mirrorOf>
    <name>cxmaven</name>
    <url>https://maven.imcaoxuan.top:8443/repository/maven-public</url>
</mirror>
```

### gradle 配置

在 build.gradle 文件中加入以下代码：
```
allprojects {
    repositories {
        maven {
            url "https://maven.caoxuan.top:8443/repository/maven-public/"
            credentials {
                username "public"
                password "public"
            }
        }
        mavenLocal()
        mavenCentral()
    }
}
```
或在 ~/.gradle/init.gradle 文件中加入以下代码：
```
allprojects {
    repositories {
        maven {
            url "https://maven.caoxuan.top:8443/repository/maven-public/"
            credentials {
                username "public"
                password "public"
            }
        }
        mavenLocal()
        mavenCentral()
    } 
    buildscript { 
        repositories {
            maven {
                url "https://maven.caoxuan.top:8443/repository/maven-public/"
                credentials {
                    username "public"
                    password "public"
                }
            }
            mavenLocal()
            mavenCentral()
        }
        
    }
}
```





