To build a hackintosh, we basically need to:

1. Build a machine with Pear-like models of hardware: Intel CPUs, AMD Polaris/Navi Graphics Card, Broadcom Wi-Fi & Bluetooth combo chipset, etc.
1. Get a bootloader for macOS: Clover bootloader or OpenCore bootloader.
1. Get a macOS latest version installer and burn it to a flash drive using a real Macintosh.
1. Fine-tune the config.plist file.
1. Startup and install the OS
1. Spoof the system and pretend to be a real Macintosh.

You miss the last step to make it work like a charm.
1. Use the _macserial.sh_ to generate some real serial numbers of the machine and its motherboard. Write them into the config.plist in the ESP.
2. Use the _hacktool_ app to locate the NIC and assign it to the en0 in order to enable the Messenger and FaceTime to work like on a real Mac.
