.. 基线检查工具 documentation master file, created by
   sphinx-quickstart on Fri Dec 10 11:33:13 2021.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Welcome to 基线检查工具's documentation!
========================================

.. toctree::
   :maxdepth: 2
   :caption: Contents:

安装使用说明：
---------------

* 基于开源项目开发的基线检查展示及docx报告生成工具。

服务器硬件绑定
----------------
* 为防止软件外泄，安装前在本机（实体机）上运行机器硬件信息检查工具（pc_info.exe或者linux_info)，生成一串机器硬件信息码。
* 将此码交给公司软件开发编译人员，编译生成该台设备专用安装包。其他设备无法打开工具。

运行
-------
* 打开软件文件夹，运行run.exe，输入服务运行的ip,端口。此ip，端口要与被检查机处于同一网段，否则检查脚本数据无法推送到本机进行处理。
* 将Agent文件夹拷贝到被检查机，以管理员权限运行基线检查脚本。
* linux运行脚本命令：
    bash linux_baseline_check.sh <ip>:<port>
* windows在powershell中运行:
    ./win2012_baseline_check.ps1
    注意执行完需要输入接收数据的ip、端口信息。

Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
