# MIUI-unbloater

### Coming soon

Rewrite to Python is coming soon. There will be dedicated .exe for Windows and executable file for Linux.

### About

This is a simple script, written in Bash, which is supposed to safely remove bloatware from Xiaomi MIUI ROM using `adb`.

### Preparing to run

Before running the script, make sure that you're phone is connected to the PC via USB cable, the USB debugging is enabled in the settings, and if you authorized your PC to use USB debugging with your phone. You can check if your phone is being detected, by using `adb devices`.
<br>
On Ubuntu-based distros, you can install `adb` using `sudo apt install adb`.
<br>
On Arch-based distros, you can install `adb` using `sudo pacman -S android-tools`
<br>
On Windows, you'll have to manually download `adb` software and usb android drivers.

#### Enabling usb debugging in MIUI

To enable USB debugging in MIUI, firstly you have to enable developer options. To do that, go to settings > about phone and click 7 times on "MIUI version". Then, go back to the settings main page, and go to advanced settings. Scroll down, and you should see developer options. Open developer options, and scroll down to "USB debugging" option. Enable it.

### Running

Just download the file from releases page, run `chmod +x MIUI-unbloater` and `./MIUI-unbloater` on your Linux distro, or via WSL (?).

### Troubleshooting

In case you're getting some errors, check whether the user you're using to run this script is inside a Linux `plugdev` group. In case it isn't, you can add your user to this group by running `sudo usermod -aG plugdev username`.
