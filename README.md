# 在联想G50-70上安装macOS
## 前言
* 因为在家闲着无聊，就决定试着在这台老设备上安装macOS。
* 由于文件太乱，所以我决定将EFI都放在[`Releases`](https://github.com/Moore2253/Install-MacOS-On-Lenovo-G50-70/releases)里，所以源代码只有`README.md`这一个文件。
* 本来想顺便写个文字安装教程，但我懒得继续写下去了，就算了吧。
## 机型配置
* 设备名：Lenovo G50-70 （20351）
* 处理器：Intel i5-4288u 双核 2.60Ghz
* 运行内存：4GB 1600Mhz DDR3
* 当前安装的Windows版本：Windows11 21h2 22000.258
* 当前安装的macOS版本：macOS Big Sur 11.6.1
* 当前使用的引导版本：
* 声卡：Conexant SmartAudio HD
* 无线网卡：QualcommAtheros AR956x Wireless Network Adapter 
* 有线网卡：Realtek PCIe GBE Family Controller (RTL8168)
* 核显卡：Intel Iris Graphics 5100 1536MB
* 独显卡：AMD redeon HD 8500M / R5 M230
* 蓝牙：Qualcomm Atheros AR3012 Bluetooth 4.0
* 硬盘：WDC WD5000LPCX-24C6HT0
## 更新随笔
* 2021年11月 配置基本完工，再次升级OpenCore，bug fix。
* 2021年10月 继续完善和升级OpenCore，重新注入三码，新增一些可以驱动的kext，修复引导的一些bug。
* 2021年9月 我在GitHub查找同机型的efi时看到[`@mirifi2k`](https://github.com/mirifi2k/)的[这篇文章](https://www.tonymacx86.com/threads/guide-lenovo-g50-80-80l0-and-catalina-10-15-2.288303/)使用`OpenCore`引导了Mac，然后我将它下载下来进行测试，发现能正常引导我的Mac，并且一部分硬件已经驱动，所以我在此efi基础上加以修改，使其能更完美的使用OpenCore引导我这台Hackintosh。
* 2021年8月 再次尝试更新，更新很成功，升级Clover，修复一些失效的驱动，修复和添加ACPI。
* 2021年7月 尝试更新Big Sur，但出现了一些问题，放弃更新继续优化Clover。
* 2021年6月 配置有了一些进展，网络、声音、显示等基本正常，升级到Catalina，日用基本OK。
* 2021年5月 首次接触macOS Mojave和Clover，对其进行配置。
## kext驱动
* 我目前使用OpenCore引导的驱动为18个，均为最新版。
### 使用驱动的硬件以及其所需`kext`驱动
* ...（下次更新）
