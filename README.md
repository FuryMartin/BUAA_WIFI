# 北航Wifi自动认证脚本

## 说明

项目Fork自：https://github.com/huxiaofan1223/jxnu_srun

原理请参考：https://blog.csdn.net/qq_41797946/article/details/89417722

我修改了相关url以适配北航wifi。

特别感谢原作者 [@huxiaofan1223](https://github.com/huxiaofan1223) 。

## 如何使用

1.下载所有文件并解压，进入`buaa_wifi.py`所在目录

2.打开`buaa_wifi.py`,分别修改第92、93行引号内的内容为你的账号和密码

3.运行，有两种方式可选。

(1)打开cmd，进入当前目录，执行以下代码
~~~
pip install -r requirements.txt
python buaa_wifi.py
~~~
(2)直接双击wifi.bat


执行完毕，校园网已成功连接

## 高级使用：电脑解锁时自动连接wifi

仅以Windows为例：

1.按键盘上的`win`键，直接打字搜索"任务计划程序"并打开

2.点击"任务计划程序"窗口右上角的`创建任务`

3.勾选`常规-不管用户是否登录都要运行`

4.点击`触发器-新建`，将`开始任务`下拉选择`工作站解锁时`

5.点击`操作-新建`，点击`浏览`，将程序路径设置为`wifi.vbe`的绝对路径

6.取消勾选`条件-只有在计算机使用交流电源时才启动此任务`

7.点击`确定`

此后脚本会在每次解锁桌面时运行一次，确保校园wifi的持续连接

## 适用场景

1.树莓派等开发板开机直连北航wifi

2.支持Shell的路由器直连北航wifi

3.部分网卡型号的电脑在锁屏后会断连wifi，此脚本可以自动重新连接wifi

4.避免每次开机都要登一遍认证账号
