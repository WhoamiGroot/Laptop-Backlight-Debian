# Laptop-Backlight-Debian
This is are the right and usefull settings for when Tuxedo doesn't work.

On Ubuntu/Debian, try changing the GRUB_CMDLINE_LINUX_DEFAULT line in /etc/default/grub to:
```
GRUB_CMDLINE_LINUX_DEFAULT="quiet splash acpi_os_name=Linux acpi_osi=! acpi_osi=Linux acpi_backlight=vendor modprobe.blacklist=nouveau"
```
This should enable the keyboard backlight key combinations (Fn /, Fn *, Fn -, Fn +).

Edit: Don’t forget to ```sudo update-grub``` and reboot after editing the file.
