# 使用nodejs服务器解析路由
url可获取任何数据，mock数据与前端交互

### 代码分析
开头顶部的模块：
```js
var http = require('http')//主要用于搭建http服务

var path = require('path')//可简化路径相关操作

var fs = require('fs')//提供本地文件的读写能力

var url = require('url')//用于生成和解析url
```
```js
http.createServer(function (req, res){
                    ·
                    ·
                    ·
                    ·   
}).listen(8800)
```
流程：
```
创建模块--> 创建server--> server函数返回一个操作对象--> 调用并启动端口为8800的服务器
```
当访问static下的html、css、图片或者直接调取请求模块，都能获取相应的内容。