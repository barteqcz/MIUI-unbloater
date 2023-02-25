# MIUI-unbloater

This is a simple script, written in Bash, which is supposed to safely remove bloatware from Xiaomi MIUI ROM using `adb`.

### Preparing to run

Before running the script, make sure that you're phone is connected to the PC via USB cable, the USB debugging is enabled in the settings, and if you authorized your PC to use USB debugging with your phone. You can check if your phone is being detected, by using `adb devices`.

On Ubuntu-based distros, you can install `adb` using `sudo apt install adb`.
On Windows, you'll have to manually download `adb` software and usb android drivers.
