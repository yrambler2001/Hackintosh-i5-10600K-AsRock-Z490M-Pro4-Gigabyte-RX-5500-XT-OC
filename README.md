# Hackintosh-i5-10600K-AsRock-Z490M-Pro4-Gigabyte-RX-5500-XT-OC
Big Sur
# Info PC

```
MB: AsRock Z490M Pro4 $158
CPU: Intel Core i5-10600K $250
VGA: Gigabyte RX 5500 XT OC 8GB $250
RAM: 32GB HyperX DDR4 16GB+16GB 3600Mhz FURY Black $210
SSD: Samsung 970 EVO 500GB (OSX) $85
SSD: Samsung 970 EVO 1TB (Windows) $160
SSD: Samsung 860 EVO 500GB
Bluetooth & Wi-Fi: Fenvi FV-T919 $50
Case: Deepcool KENDOMEN RD $60
PSU: Chieftec BDF-600S 600W $60
Cooler: be quiet! Dark Rock 4 $90
```

# Hackintosh + OpenCore (Supported version: 0.6.7)

- https://dortania.github.io/OpenCore-Desktop-Guide

# Works

- Audio
- HDMI Audio
- Ethernet
- Bluetooth
- GPU
- USB ports
- Switch between Windows and MacOS with [rEFInd bootloader](https://github.com/agners/rEFInd) [(website)](https://www.rodsbooks.com/refind/) using mouse. 

If you prefer to use only OpenCore without rEFInd, please remove these lines:
```
<key>LauncherPath</key>
<string>\refind\refind_x64.efi</string>
```

# Result

![Info](/images/info.png)
![SSD](/images/ssd.png)

Geekbench 5 https://browser.geekbench.com/v5/cpu/6944941

# Note

The file config.plist. Please change MLB, SystemSerialNumber, SystemUUID into your code

```
<dict>
		<key>AdviseWindows</key>
		<true/>
		<key>MLB</key>
		<string>xxxxxxxxxxxxxxx</string>
		<key>ROM</key>
		<data>Z0SJO6Bu</data>
		<key>SpoofVendor</key>
		<true/>
		<key>SystemProductName</key>
		<string>iMac20,1</string>
		<key>SystemSerialNumber</key>
		<string>xxxxxxxxxxx</string>
		<key>SystemUUID</key>
		<string>xxxxxxxx-xxxxx-xxxxx-xxxx-xxxxxxxx</string>
		<key>SystemMemoryStatus</key>
		<string>Auto</string>
</dict>
```
