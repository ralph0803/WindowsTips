# WindowsTips

kernel.dll内置了P2P加速功能，如果你不打算使用P2P加速，可以删掉这个DLL，但是删掉的同时也必须要删掉kernelUpdate.exe

### 蓝屏

可以在计算机右键属性中的“系统失败”的选项中，把dump文件写入开启。会在c:\windows\MiniDump的文件夹里面，对于每一次蓝屏都有记录。打开dump文件需要特定的工具，叫做debugging tool，是微软自己出品的。打开debugging tool后，将相应的dump拖进去查看

