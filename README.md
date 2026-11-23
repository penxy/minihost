# Minihost

基于 LEDE/OpenWrt 的树莓派 4B 固件。

## 效果图片

* [更多效果图片](README_MORE.md)

## 项目功能

1. 软路由：openclash代理，DNS服务器，LuCI 管理后台。
2. NAS：USB3.0转SATA机械硬盘，FTP/Samba 文件协议。
3. Docker：一键部署：Nextcloud、Hugo、Navidrome、Vaultwarden、deepseek-ai-h5、QQ AI等。
4. 屏幕显示(OLED SH1106 128×64): 时间、CPU 温度、CPU 使用率、内存使用率。
5. 屏幕显示(HDMI 1024×600 Qt6): 壁纸、天气、音乐、Docker 容器状态、语音控制、硬盘SMART、图片幻灯片。
6. 风扇温控(一路继电器 GPIO27)：按CPU温度/HDD温度执行 启动/关闭。
7. 交互控制(vosk本地识别)：支持语音/MQTT 控制屏幕显示页面。 
8. 个人网站：nginx 按子域名反向代理各Docker镜像端口，并通过frpc内网穿透到公网域名。
9. 其它：定时关闭耗能大的服务、日志规范、ACME自动续期HTTPS证书等。

## 硬件设备

* [详见](https://gitlab.com/xuanyu2/hardware)

## 代码仓库

* [Minihost](https://gitlab.com/xuanyu2/minihost)

## Q&A

* 为什么做这个项目？
* 在9月底的时候看到了 [B站UP主狐冥栎的迷你机箱](https://www.bilibili.com/video/BV1V7tN65E1H/?spm_id_from=333.1007.top_right_bar_window_default_collection.content.click&vd_source=599f3be0badae3fe83d3b0e57d83bc79) ，同时手里还有块树莓派4B，然后决定做的。
