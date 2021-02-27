# OpenCore (0.6.6) EFI for B360

### Version 2.1.1

**CPU**: Intel i5-8600 (3,10GHz, 6 cores - 6 threads)

**GPU**: ASUS ROG STRIX Radeon RX 570 8GB VRAM

**RAM**: (2 x 4GB) HyperX Fury 2666MHz & (2 x 4GB) Ballistix Sport 2666MHz

**Storage**: Kingston 120GB SSD

**Motherboard**: MSI B360M Bazooka

**Ethernet**: Realtek 1 Gigabit Ethernet Controller

**Audio**: Realtek ALC887 Codec/Apple Inc. USB-C to Headphone Jack Adapter

_Configured for MSI B360M Bazooka Motherboard_

![proof](https://i.ririxi.dev/macos_new.png)

# Updates

- 2.1.1
  - Update Picker resources to [LuckyCrack's Dark Theme](https://github.com/LuckyCrack/OpenCore-Themes)
  - Change PickerVariant to `Auto`.
- 2.1.0
  - Update to OpenCore 0.6.6
  - Update **Lilu, WhateverGreen, AppleALC, VirtualSMC** kexts.
  - Remove BootProtect key and change it to LauncherOption (OpenCore 0.6.6 change).
- 2.0.1
  - Change BootProtect to `Bootstrap` value.
- 2.0
  - Update to OpenCore 0.6.5.
  - Update **Lilu & WhateverGreen & AppleALC** kexts.
  - Add forgotten CPUFriend kext.

# FAQ
___Q: Why ``MacPro7,1`` SMBIOS?___

A: On this SMBIOS we are getting iServices out-of-box without any issues etc. People will say that Power Management for my CPU can be borked on this SMBIOS but it isn't since I'm patching it with CPUFriend kext.

___Q: Why my USB ports doesn't work?___

A: You should patch your USB ports by yourself with [USBMap python script](https://github.com/CorpNewt/USBMap) and just replace my USBMap.kext with your generated.

___Q: Why my Power Management is borked for 8th/9th x CPU?___

A: You should check [CPUFriendFriend](https://github.com/corpnewt/CPUFriendFriend) and generate ProviderData kext and replace mine.

_DISCLAIMER: This config was made for my hardware. Everyone have different one and not always exact - so please, don't use this config as yours, but just follow [dortania guide](https://dortania.github.io/OpenCore-Install-Guide/) and inspirate with mine if you really need to._
