# ipmitool
本项目是ipmitool windows可以执行文件和相应的动态库。

* 代码版本：commit-4d4f29f
* 连接串口：
    * 配置串口输出
    ```
    # Ubuntu 20.04
    # /etc/default/grub
    GRUB_CMDLINE_LINUX="console=tty1 console=ttyS0,115200
    GRUB_TERMINAL="console serial"
    GRUB_SERIAL_COMMAND="serial --speed=115200"
    ```
    * ipmitool -H [IP] -U [USER] -P [PASSWD] -I lanplus sol activate
