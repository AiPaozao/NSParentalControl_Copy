# NSParentalControl_Copy
Original author's repository address: https://github.com/TristanIsrael/NSParentalControl This is a parental control plugin that runs under the Switch Atmosphere CFW system. The original author's code does not function properly on Atmosphere 1.9.5 with Switch firmware version 20.5.0. 
Using my spare time, I modified the code with the help of AI to adapt it for the 20.5.0 system. Since I don't understand code myself, I only used AI to adapt the code, and there are still many bugs in some functions. Currently, the implemented features include: setting individual time limits for each user; when the time is up, a timeout screen is displayed and will automatically close only after 5 minutes (during this period, normal gameplay is impossible as the game screen is not visible, only sound); the system no longer requires pressing the power button to reboot. After 5 minutes, the timeout screen closes, providing time for the current user to save and exit the game. If the user still hasn't exited afterwards, the timeout screen will continue to display to prevent further gameplay. This basically meets my personal usage requirements. Since I don't know how to use GitHub, I have uploaded all the modified code and the compiled plugin as a compressed file to GitHub. Everyone is welcome to download and improve it freely.

The code has been localized using AI, with the default language set to Chinese. Users can choose to switch to English in the plugin's settings, but this feature has not been tested.

Here, I would like to express my heartfelt gratitude to the original author.
-------------------------------------------------------------------------------
Installation

Install the required Tesla Menu or Ultrahand Overlay.

⚠️ If you want notifications you have to install Ultrahand Overlay. Please look at its documentation to know how to install it and how to enable the notifications.

Download the latest release from GitHub.

The sysmodule is provided as a ZIP file which can be directly unzipped in the folder /atmosphere/contents/

Here are the files and their destination:

File-----------------------Destination------------------------------------------------description

exefs.nsp----------------/atmosphere/contents/4200000000003103--------------The core of the system as a sysmodule

toolbox.json-------------/atmosphere/contents/4200000000003103--------------A description file for Atmosphère

boot2.flag---------------/atmosphere/contents/4200000000003103/flags--------Mandatory file to make the sysmodule start at boot

parental_control.ovl-----/switch/.overlays-------------------------------------------The overlay

After copying the files, reboot the console.


原作者仓库地址：https://github.com/TristanIsrael/NSParentalControl 这是一个在SWITCH大气层系统下运行的一个家长控制插件，原作者的代码在大气层1.9.5，SWITCH固件版本20.5.0下无法正常工作，自己用业余时间通过AI对代码进行了修改，适配了20.5.0系统，由于自己不懂代码，只是用AI对代码做了适配，部分功能仍存在很多BUG。目前实现的功能是：对每个用户单独设置限制时间，时间到了后显示超时屏幕且5分钟后才会自动关闭（在这期间无法正常进行游戏，因为看不到游戏画面，只有声音），不再通过按开机键进行重启，5分钟后超时屏幕关闭，中间有时间让当前用户保存和退出游戏，之后如果用户仍未退出，则继续显示超时屏幕来阻止用户进行游玩，基本满足了我个人的使用要求。由于我不会用GITHUB，将所有更改后的代码和编译后的插件压缩后上传到了GITHUB，大家可以随意下载和优化。
用AI对代码进行了汉化，默认为中文语言，插件中添加了语言选项，可选英文。
安装方法参照原作者的即可。

测试平台：
SWITCH固件版本20.5.0
大气层系统版本1.9.5
特斯拉插件采用的是Ultrahand 版本2.2.7
nx-ovlloader 版本2.0.0

Ultrahand仓库地址：https://github.com/zdm65477730/Ultrahand-Overlay
nx-ovlloader的仓库地址：https://github.com/ppkantorski/nx-ovlloader

编译环境搭建参考GBATEMP论坛中的作者Impeeza：https://gbatemp.net/threads/setup-a-devkitpro-environment-on-windows.652238/
https://gbatemp.net/threads/install-msys-environment.652234/
