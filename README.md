# NSParentalControl_Copy
Original author's repository address: https://github.com/TristanIsrael/NSParentalControl This is a parental control plugin that runs under the Switch Atmosphere CFW system. The original author's code does not function properly on Atmosphere 1.9.5 with Switch firmware version 20.5.0. 
Using my spare time, I modified the code with the help of AI to adapt it for the 20.5.0 system. Since I don't understand code myself, I only used AI to adapt the code, and there are still many bugs in some functions. Currently, the implemented features include: setting individual time limits for each user; when the time is up, a timeout screen is displayed and will automatically close only after 5 minutes (during this period, normal gameplay is impossible as the game screen is not visible, only sound); the system no longer requires pressing the power button to reboot. After 5 minutes, the timeout screen closes, providing time for the current user to save and exit the game. If the user still hasn't exited afterwards, the timeout screen will continue to display to prevent further gameplay. This basically meets my personal usage requirements. Since I don't know how to use GitHub, I have uploaded all the modified code and the compiled plugin as a compressed file to GitHub. Everyone is welcome to download and improve it freely.

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
