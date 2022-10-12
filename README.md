NOT UPDATED ANYMORE DUE TO ME CONVERTING THIS INTO A NAS

It was a good run :)

# Intel Hackintosh (Opencore)
- Intel Core 2 Quad Q8200
- Gigabyte GA-EP45-UD3R (rev 1.1)
- Corsair XMS2 DDR2-800 8GB (4x2GB)
- Gigabyte GT 710 GDDR3 1GB
- ASUS BT400 Bluetooth
- Opencore 0.6.8
- macOS Big Sur 11.2.3

# What doesn't work normally
- DRM in Safari and Apple TV+
- AirDrop
- Gaming (Seriously don't use this for gaming)
- Booting versions below 10.12 (not working on that as of right now)

# Tested macOS versions that works
- Big Sur (need to have working emulated NVRAM, more notes below)
- Catalina
- Mojave
- Mountain Lion (boots into recovery, haven't installed)

# What doesn't work in the 11.4 Beta
- Sometimes Kernel Panics during boot (run first aid in recovery to fix)
- Shut down from macOS doesn't fully power off the system and put the system into deep sleep

# Additional Notes
- Change the serial and stuff if you're using this EFI
- You might want to change the USBMap.kext to USBInjectAll.kext or compile your own USBMap.kext when booted into macOS
- Emulated NVRAM IS REQUIRED for every Big Sur update, for other versions, it's not needed at all

# Future additions and testing
- Converting EFI for use on Pre-macOS (will be put in a different repository, currently on hold)
- trying to update the EFI to Opencore 0.6.9

# For use in Big Sur (Methods given by TheBloke: https://github.com/TheBloke)
- Must have working NVRAM (https://dortania.github.io/OpenCore-Post-Install/misc/nvram.html)
- Method to do a fresh install from USB: https://www.tonymacx86.com/threads/x299-big-sur-support.302143/page-107#post-2203225
- Method to upgrade from Catalina to Big Sur: https://www.insanelymac.com/forum/topic/345910-unable-to-upgrade-from-catalina-to-big-sur-on-system-with-legacy-bios/?tab=comments#comment-2746083
- The config.plist got both methods covered except for making the nvram.plist, so I recommend installing Catalina first and making the NVRAM work from there
