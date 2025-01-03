## Gentoo Linux Kernel Configuration on Lenovo Thinkpad P1 Gen5

1. Output from lspci on Lenovo Thinkpad P1 Gen5 and
1. Linux kernel configuration for linux-6.6.67-gentoo.



配置文件是在**gentoo-kernel-bin** 的环境下，使用 `make localmodconfig` 生成的配置文件，并在`genkernel --menuconfig --oldconfig all`中多次根据`dmesg -lerr`的输出调整确定的。



目前还`dmesg`有一个错误：

```
ucsi_acpi USBC000:00: UCSI_GET_PDOS failed (-95)
```

还没有找到解决方法，但不影响正常使用。
