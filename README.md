# WCH-Link Firmware

Source: [WCH-LinkUtility](https://www.wch.cn/downloads/WCH-LinkUtility_ZIP.html)

Firmware list

* WCH-Link
* WCH-LinkE
* WCH-LinkW
* WCH-DAPLink

Current firmware version: 2.19 (aka. v39).
> NOTE: The firmware version is not the same as the version shown by WCH's toolchain. Because WCH calculates the version number by major * 10 + minor, so the firmware version 2.10 is actually v30 0x020a.

## Flash firmware command (wlink)

wlink: https://github.com/ch32-rs/wlink

Flash another WCH-LinkE example:

Remember to run on IAP mode.

```bash
wlink unprotect
wlink erase
wlink flash ./WCH-LinkE-APP-IAP.bin
```

Upgrade self example:

```bash
wlink upgrade ./FIRMWARE_CH32V305.bin
```
