## 教程：红米Note 7刷入Sailfish OS 3、Ubuntu Touch

### 先决条件

* 非日常主力机的红米Note7一部，确保电量充足、已经解锁，并且成功刷入第三方Recovery，例如`Twrp`或`OrangeFox`
* 能够联网下载文件，并且能把文件拷贝到红米Note7的设备，例如，你可以用手机下载，通过OTG连接你的红米Note7，或者通过一台电脑、一根USB C2C或A2C的数据线拷贝数据

### 刷入Sailfish OS

* 下载必要的两个文件，从[这里](https://github.com/sailfish-lavender/builds/releases)下载`@Danct12`编译的红米Note7的专属`Lineage 16基础包`和最新的`Sailfish OS系统包`
* 确保你有`lineage-16.0-20200107-unofficial-lavender.zip`和`sailfishos-3.2.1.20-20200429-lavender-danctnix.zip`这两个文件（我这里是当前编译的版本，如果你后面看到更新的编译文件，请使用新的），关机，按住`电源键`和`音量+`，进入Recovery，将下载的文件拷贝到红米Note7中
* 执行清理操作，勾选`Dalvik/ART Cache`、`Cache`、`System`、`Vender`、`Data`并清理。（执行清理操前如有需要请先备份分区）
* 依次刷入`Lineage 16基础包`和`Sailfish OS包`，刷写成功后重启手机即可进入Sailfish OS

### 刷入Ubuntu Touch

- 下载必要的三个文件，从[这里](https://build.lolinet.com/file/halium/GSI/ubports_GSI_installer_v9.zip/)下载通用的`Ubuntu Touch GSI系统包`，从[这里](https://build.lolinet.com/file/lineage/lavender/lineage-16.0-20200226-UNOFFICIAL-lavender.zip)下载红米Note7的专属`Lineage 16基础包`，从[这里](https://github.com/ubports-lavender/ubports-ci/releases)下载`@Danct12`编译的红米Note7的专属`halium-boot`启动文件
- 确保你有`ubports_GSI_installer_v9.zip`和`lineage-16.0-20200226-UNOFFICIAL-lavender.zip`和`halium-boot.img`这三个文件（我这里是当前编译的版本，如果你后面看到更新的编译文件，请使用新的），关机，按住`电源键`和`音量+`，进入Recovery，将下载的文件拷贝到红米Note7中
- 执行清理操作，勾选`Dalvik/ART Cache`、`Cache`、`System`、`Vender`、`Data`并清理。（执行清理操前如有需要请先备份分区）
- 依次刷入`Lineage 16基础包`和`halium-boot启动镜像`，最后刷入`ubuntu touch gsi系统包`，刷写成功后重启手机即可进入Ubuntu Touch，默认的密码是`phablet`

### 感谢
* 我只是个搬运工，感谢`@Danct12`和`@erfanoabdi`两位真正的开发者大佬。我的愿景是希望能在手机上运行Arm64 Docker，然后把闲置手机作为一个真正的ARM服务器，毕竟现在是个手机性能比树莓派都好，还不用额外配显示器。
