# 在联想G50-70上安装macOS
## 前言
* 因为今年暑假闲着无聊，就翻出了家里这台闲置机器，刚好前几个月听说了黑苹果这个玩意，并且听说挺难整，决定试着安装。
* 由于文件太乱，所以我决定将EFI都放在[`Releases`](https://github.com/Moore2253/Install-MacOS-On-Lenovo-G50-70/releases)里，所以源代码只有`README.md`这一个文件。
* 本来想顺便写个文字安装教程，但我懒得继续写下去了，就算了吧。
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
## 引导
* 目前我都使用`CLOVER`引导，最新版为`5139`，但我目前使用`5138`。
## 驱动`kext`
* 我目前使用的驱动为17个，均为最新版。`Releases`>`Downloadv1.0`中的三个efi的压缩中的`kexts`有二三十来个，我已经在陆续删除无用驱动，避免启动过慢、efi过于臃肿。
### 已驱动的硬件以及其所需`kext`驱动
* ...（下次更新）
