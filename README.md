# 北航Wifi自动认证脚本

## 说明

项目Fork自：https://github.com/huxiaofan1223/jxnu_srun

我修改了相关url以适配北航wifi。

特别感谢原作者 [@huxiaofan1223](https://github.com/huxiaofan1223) 。

## 如何使用

1.下载所有文件并解压，进入`buaa_wifi.py`所在目录

2.打开`buaa_wifi.py`,分别修改第92、93行引号内的内容为你的账号和密码

3.打开cmd，进入当前目录，执行以下代码

~~~
pip install -r requirements.txt
python buaa_wifi.py
~~~

执行完毕，校园网已成功连接

## 适用场景

1.树莓派等开发板开机直连北航wifi

2.支持Shell的路由器直连北航wifi
