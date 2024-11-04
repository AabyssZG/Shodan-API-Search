![Shodan-API-Search](https://socialify.git.ci/AabyssZG/Shodan-API-Search/image?description=1&font=KoHo&forks=1&issues=1&language=1&logo=https%3A%2F%2Favatars.githubusercontent.com%2Fu%2F54609266%3Fv%3D4&name=1&owner=1&pattern=Floating%20Cogs&pulls=1&stargazers=1&theme=Dark)

## ✈️ 一、工具概述

在查询国外资产的过程中，发现Shodan测绘引擎的API调用并不方便，且网上没有相应的脚本（有些老的脚本基于Python2）

于是基于Python3，将Shodan API的查询进行了重写，并提供了多个参数便于使用和导出数据

如果师傅们觉得好用，欢迎给本项目点个Star，万分感谢~❤️

## 🚨 二、安装Python依赖库

```
pip install shodan
```

## 🐉 三、工具使用

### 3.1 查询指定语句并导出

比如想要查询 `port:22` 这个测绘语句，找到200个资产（一页是100个资产），并导出为 `output.txt`：

```
python3 Shodan-API-Search.py -k <Shodan API Key> -s port:22 -p 2 -o output.txt
```

### 3.2 查询指定IP的信息

比如想要查询 `1.1.1.1` 这个IP的资产测绘信息：

```
python3 Shodan-API-Search.py -k <Shodan API Key> -i 1.1.1.1
```