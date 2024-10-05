# WCH-Link Firmware

Source: [WCH-LinkUtility](https://www.wch.cn/downloads/WCH-LinkUtility_ZIP.html)

Firmware list

* WCH-Link
* WCH-LinkE
* WCH-LinkW
* WCH-DAPLink

Current firmware version: 2.14 (aka. v34).
> NOTE: The firmware version is not the same as the version shown by WCH's toolchain. Because WCH calculates the version number by major * 10 + minor, so the firmware version 2.10 is actually v30 0x020a.

## Flash firmware command (wlink)

wlink: https://github.com/ch32-rs/wlink

Flush WCH-LinkE example:

Remember to run on IAP mode.

```bash
wlink unprotect
wlink erase
wlink flush ./WCH-LinkE-APP-IAP.bin
```
