# 在联想G50-70上安装macOS
## 前言
* 因为在家闲着无聊，就决定试着在这台老设备上安装macOS。
* 由于文件太乱，所以我决定将EFI都放在[`Releases`](https://github.com/Moore2253/Install-MacOS-On-Lenovo-G50-70/releases)里，所以源代码只有`README.md`这一个文件。
* 本来想顺便写个文字安装教程，但我懒得继续写下去了，就算了吧。
## 机型配置
* 设备名：Lenovo G50-70 （20351）
* 处理器：Intel i5-4288u 双核 2.60Ghz
* 运行内存：4GB 1600Mhz DDR3
* Windows版本（当前安装）：Windows11 21h2 22000.258
* macOS版本（当前安装）：macOS Big Sur 11.6.1
* 声卡：Conexant SmartAudio HD
* 无线网卡：Qualcomm Atheros AR956x Wireless Network Adapter 
* 有线网卡：Realtek PCIe GBE Family Controller (RTL8168)
* 核显卡：Intel Iris Graphics 5100 1536MB
* 独显卡：AMD redeon HD 8500M
* 蓝牙：Qualcomm Atheros AR3012 Bluetooth 4.0
* 硬盘：WDC WD5000LPCX-24C6HT0
## 引导
* `OpenCore076` 或 `Clover5138`
* 2021年10月
* 2021年9月 我在GitHub查找同机型的efi时看到[`@mirifi2k`](https://github.com/mirifi2k/)的[这篇文章](https://www.tonymacx86.com/threads/guide-lenovo-g50-80-80l0-and-catalina-10-15-2.288303/)使用`OpenCore`引导了Mac，然后我将它下载下来进行测试，发现能正常引导我的Mac，并且一部分硬件已经驱动，所以我在此efi基础上加以修改，使其能更完美的使用OpenCore引导我这台Hackintosh。
* 2021年5月 首次接触Hackintosh和Clover，对其进行配置。
## kext驱动
* 我目前使用OpenCore引导的驱动为18个，均为最新版。
### 使用驱动的硬件以及其所需`kext`驱动
* ...（下次更新）
