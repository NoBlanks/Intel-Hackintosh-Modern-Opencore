# Intel Hackintosh (Opencore)
- Intel Core 2 Quad Q8200
- Gigabyte GA-EP45-UD3R (rev 1.1)
- Corsair XMS2 DDR2-800 8GB (4x2GB)
- Gigabyte GT 710 GDDR3 1GB (alt card: XFX 9600 GSO 768MB)
- ASUS BT400 Bluetooth
- Opencore 0.6.8
- MacOS Big Sur 11.4 Beta 1 (Very unstable)

# What doesn't work normally
- DRM in Safari and Apple TV+
- AirDrop
- Gaming (Seriously don't use this for gaming)
- Booting versions below 10.12 (working on that right now)

# What doesn't work in the 11.4 Beta
- Sometimes Kernel Panics during boot (run first aid in recovery to fix)
- Shut down from macOS doesn't fully power off the system and put the system into deep sleep

# Additional Notes
- Change the serial and stuff if you're using this EFI
- You might want to change the USBMap.kext to USBInjectAll.kext or compile your own USBMap.kext when booted into macOS
- Yes this EFI has emulated NVRAM and IS REQUIRED for every Big Sur update, for other versions, it's not needed at all

# Future additions and testing
- Using chris1111's patchers in Mojave, Catalina and maybe Big Sur to get my Nvidia Tesla card working on those versions
- Mojave Patcher: https://github.com/chris1111/Fix-Old-NVIDIA-macOS-Mojave
- Catalina (maybe I'll test this in Big Sur too): https://github.com/chris1111/Legacy-Video-patch
- Older versions of macOS/OS X (10.4-10.11)
- Might add Inject Nvidia for older cards
