# WindowsTips

kernel.dll内置了P2P加速功能，如果你不打算使用P2P加速，可以删掉这个DLL，但是删掉的同时也必须要删掉kernelUpdate.exe

### 蓝屏

可以在计算机右键属性中的“系统失败”的选项中，把dump文件写入开启。会在c:\windows\MiniDump的文件夹里面，对于每一次蓝屏都有记录。打开dump文件需要特定的工具，叫做debugging tool，是微软自己出品的 (`https://dl.pconline.com.cn/download/896557.html`)。打开debugging tool后，将相应的dump拖进去查看

### 蓝屏 代码 7B
深度学习机器是用MSI Z370 A PRO的主板，在主板官网上面有BIOS的升级zip文件，按照相应的教程解压到U盘里面（现在WCNC的那个U盘是有这些BIOS的）。然后就进行BIOS升级，但升级完后，会出现windows进不去的问题，蓝屏代码**7B**。后来查了查网上，是因为SATA硬盘的启动模式设置的问题，在MSI的BIOS设置中(del键进去)，右上角搜索，搜索SATA，会出现AHCI mode，此时应替换到optane mode的就可以了。
