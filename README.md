# 说明
/etc/hosts 添加如下代码
127.0.0.1 frank.com
127.0.0.1 jack.com

运行命令:
PORT=8001 node server.js
PORT=8002 node server.js

浏览器分别输入:
frank.com:8001
jack.com:8002

在frank.com(跨域)中点击按钮, 可以看到控制台会有输出信息.
因为是index.html中跨域到jack.com, 所以从jack.com中点击按钮(此时没有跨域)会得到一样的结果.
