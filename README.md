#### Magisk WIFI Bonding

在「高通设备」上以40Mhz运行2.4Ghz/5.0Ghz的Wifi。

#### 说明

请按照以下说明进行操作@axeldna:

1. 移除已安装了的WIFI Bonding模块。
2. 移除所有已保存的2.4Ghz的Wifi（删不删都可以，非必要）
3. 重启手机（以确保从云服务中删除相关的Wifi设置项）。
4. 安装Wifi Bonding模块。
5. 重启手机（根据Magisk指示来重启）。
6. 试着开始接入2.4Ghz的Wifi。
7. 自测新连上的2.4Ghz的Wifi有150Mbps的连接速度。


该模块适用于绝大多数设备。  
一般来说，设备都会提供一个ini文件来控制Wifi行为。  
该模块的原理很简单，就是修改了`WCNSS_qcom_cfg.ini`这个文件以支持40mhz。  
但并非所有设备都需要该模块。  
如果您在系统分区中找到`WCNSS_qcom_cfg.ini`，并且在使用过程中发现问题，那么你可以新建一个issue来向我反馈；  
如果找不到这个文件，那么该模块则不支持该设备，同时也不支持大部分的Nexus / Pixel设备。

#### 注意

* 您应该使用最新的Magisk Manager来安装此模块。如果您遇到Magisk Manager安装中的任何问题，请尝试使用Recovery来安装它。
* 最近修复的项目：
添加更多文件路径（/verdor）

#### 所有权 以及 支持

* 版权所有 (C) 2017 simonsmh <simonsmh@gmail.com>
* 欢迎提交任何issue以及Pull Request。
* 你可以在这个地址star该模块 [GitHub](https://github.com/Magisk-Modules-Repo/magisk-wifi-bonding).
