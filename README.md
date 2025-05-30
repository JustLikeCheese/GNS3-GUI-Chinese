GNS3-gui 汉化版
========

GNS3 GUI 汉化版仓库。欢迎大家提交 commit。

安装
------------

请参考 <https://docs.gns3.com/>

依赖的软件包
---------------------

有些 Linux 发行版已经内置了 PyQt5（当然你也可以通过 PyPi 来安装）。
其他 Python 依赖项会在 GNS3 GUI 安装过程中自动安装，并且已列出。

要通过 Telnet 连接节点，必须安装 Telnet 客户端。在 Linux 系统中，这通常包括一个终端模拟器（如 xterm、gnome-terminal 或 konsole）以及 telnet 程序。若需通过图形用户界面连接节点，则需要安装VNC客户端，或者可选择使用 SPICE 客户端以连接 Qemu 节点。


在 GNS3 中使用数据包捕获功能时，建议安装Wireshark。

开发
-----------

如果您想更新界面，可以使用 QT 工具修改 .ui 文件。然后执行以下操作：

``` {.bash}
cd scripts
python build_pyqt.py
```

### 调试

如果您想在内部 shell 中查看完整的日志，可以输入：

``` {.bash}
debug 2
```

或者使用调试标志启动应用程序，即添加 --debug 参数。

由于PyQT会拦截调试，您可以使用一个网页调试器来检查内容，比如：<https://github.com/Kozea/wdb>