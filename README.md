# 在联想G50-70上安装macOS
## 前言
* 因为今年暑假闲着无聊，就翻出了家里这台闲置机器，刚好前几个月听说了黑苹果这个玩意，并且听说挺难整，决定试着安装。
* 由于文件太乱，所以我决定将EFI都放在[`Releases`](https://github.com/Moore2253/Install-MacOS-On-Lenovo-G50-70/releases)里，所以源代码只有`README.md`这一个文件。
* Tips：因为我编辑这个`README.md`时已经开学，所以每天只能更新一点点，敬请谅解。
## 机型配置
* 设备名：Lenovo G50-70 （20351）
* 处理器：Intel i5-4288u 四核（Mac显示双核）2.60Ghz
* 运行内存：4GB 1600Mhz DDR3
* Windows版本（当前安装）：Windows10 21h1
* macOS版本（当前安装）：macOS Big Sur 11.6
* 声卡：Conexant SmartAudio HD
* 无线网卡：Qualcomm Atheros AR956x Wireless Network Adapter 
* 有线网卡：Realtek PCIe GBE Family Controller (RTL8168)
* 核显卡：Intel Iris Graphics 5100 1536MB
* 独显卡：AMD redeon HD 8500M
* 蓝牙：Qualcomm Atheros AR3012 Bluetooth 4.0
* 硬盘：WDC WD5000LPCX-24C6HT0
## 安装macOS（文字教程）
### 需要准备
* 1，一个容量>16GB的u盘；
  * 尽量选择有品牌、传输稳定的u盘，不要选择杂牌，否则安装过程可能会卡住。
* 2，一个黑苹果镜像；
  * 可以通过[`黑果小兵部落阁`](https://blog.daliansky.net/)及其微信公众号下载，其它下载镜像站点自行百度。
* 3，一台联想G50-70电脑；
  * Windows、Linux均可；
  * 需要安装有[`balenaEtcher`](https://www.balena.io/etcher/)。
### 开始安装
* 1，打开电脑上的`balenaEtcher`；
* 2，点击`Flash from file`选择你下载的镜像`macOS Big Sur 11.5.2 20G95 Installer for OpenCore 0.7.1 and CLOVER 5138 and PE.dmg`（文件名类似）；
* 3，点击`Select target`选择你要刷入的u盘；
* 4，点击`Flash`开始刷写（会弹出`命令提示符`获取管理员权限，请点击`“是”`）；
* 5，等待软件提示`Flash done`后，重启电脑
* 6，在`Lenovo`logo并未开始转圈或进入其它引导界面时，按下Fn+F12（亮度+键）；
* 7，你会发现有三个u盘启动项，它们分别是OC、CLOVER、PE的启动项。
  * 如果你想使用`OC`引导，你可能需要编辑`EFI/OC/config.plist`中的：
    * Kernel- Quirks- AppleXcpmCfgLock
    * UEFI- Quirks-IgnoreInvalidFlexRatio
