---
description: Some info about rooting with Magisk and installing a new custom ROM.
---

# Rooting With Magisk and Installing Custom ROMs

## Where to start? <a href="#where-to-start" id="where-to-start"></a>

All Android tablets and phones have a different method of going about rooting. You need to find a guide and instructions that are **SPECIFICALLY** for your device's model. Some manufacturers or Android phone device models make it very difficult or impossible to root or flash a custom recovery because of things like fuse checks or simply not releasing the kernel source or the ability to unlock your bootloader. All data on your Android device usually needs to be erased in this process.

## ​How to Root  <a href="#how-to-root-xda-android-forums-click-here-to-learn-about-rooting" id="how-to-root-xda-android-forums-click-here-to-learn-about-rooting"></a>

{% hint style="warning" %}
### You will need to root with [**Magisk**](https://github.com/topjohnwu/Magisk/blob/master/README.MD) in order to install Magisk modules.

### Magisk [README](https://github.com/topjohnwu/Magisk/blob/master/README.MD) and [FAQ](https://topjohnwu.github.io/Magisk/faq.html)

### Magisk [Installation Instructions](https://topjohnwu.github.io/Magisk/install.html)

#### Note: Magisk is not necessarily required. You can typically manually install or edit necessary files with other root methods such as SuperSU. Magisk just tends to be easier and is a more mainstream root method these days since installing modules is simple and can be disabled/removed if something goes wrong. KernelSU is another option that can install Magisk modules. <a href="#note-magisk-is-not-necessarily-required-you-can-typically-manually-install-or-edit-necessary-files-w" id="note-magisk-is-not-necessarily-required-you-can-typically-manually-install-or-edit-necessary-files-w"></a>
{% endhint %}

{% hint style="info" %}
### If you want to use a custom ROM for your device to try [to use amiibo](../guides/using-amiibo.md) (NFC emulation over Bluetooth) with JoyCon Droid, your custom ROM must: <a href="#if-you-want-to-use-a-custom-rom-for-your-device-to-try-to-use-amiibo-nfc-emulation-over-bluetooth-wi" id="if-you-want-to-use-a-custom-rom-for-your-device-to-try-to-use-amiibo-nfc-emulation-over-bluetooth-wi"></a>
{% endhint %}

{% hint style="info" %}
* Be **Android 9** (**P**ie) and greater.
* Be built at least until **after 2020 September 07 (All** [**LineageOS**](https://lineageos.org/) **based ROMs)**
* Have a Bluetooth HID MTU SIZE of 512 bytes. This is usually defined in the custom ROM's source code as `HID_DEV_MTU_SIZE 512` There is not a way to view this while using your device. [Here's an example!](https://github.com/crdroidandroid/android_system_bt/blob/15ef283954c79c903e393945d0bf7f2f94b8761c/internal_include/bt_target.h) \[The Patch introduced on 7th of September 2020 is only for the AOSP Bluetooth Stack. If an Android device uses the Qualcomm Bluetooth Stack, HID\_DE&#x56;_\__&#x4D;TU\_SIZE is still set to 64.]



You can find your ROM's Build date by checking the date on the ROM you flashed or going to your phone's **Settings** app → **About phone** (open **System** first on some phones) → **Android version** (open **Status** first on some phones) → **Build date**
{% endhint %}

Samsung Android devices are the only known brand that has a large enough Bluetooth HID MTU size found in the stock system firmware. This means Samsung devices usually don't need a custom ROM for amiibo emulation except if you have an older Samsung model and need to upgrade to at least Android 9.

You still need to root your Samsung or other Android device with Magisk in order to install Magisk modules. Some Samsung models are extremely difficult to root. Qualcomm Snapdragon Samsung devices of the same phone can be harder to root than Exynos Samsung devices.

OnePlus, Google Pixel, and many other phones can have simple methods and better support for rooting and flashing custom recovery like TWRP and ROMs.

{% hint style="danger" %}
#### This is all considered advanced software. No one else besides you can be responsible if you do not read everything carefully for your phone and break something. You can usually recover most devices from a softbrick if you do something wrong, but it's better to avoid that in the first place

#### Samsung phones have Knox Warranty Bit. If that's tripped from custom software, you can lose certain important functionality. <a href="#samsung-phones-have-knox-warranty-bit-if-thats-tripped-from-custom-software-you-can-lose-certain-imp" id="samsung-phones-have-knox-warranty-bit-if-thats-tripped-from-custom-software-you-can-lose-certain-imp"></a>

#### Custom ROMs and root can cause different Android devices to fail [Play Integrity](https://xdaforums.com/t/info-play-integrity-api-replacement-for-safetynet.4479337/) or [SafetyNet Attestation](https://developer.android.com/training/safetynet/attestation) checks. This can cause problems with apps like Banking apps, Google Pay, Netflix, Pokemon GO, etc. <a href="#custom-roms-and-software-can-cause-different-android-devices-to-fail-safetynet-attestation-and-not-p" id="custom-roms-and-software-can-cause-different-android-devices-to-fail-safetynet-attestation-and-not-p"></a>

You might be able to overcome those issues by using modules like [Play Integrity Fix](https://xdaforums.com/t/module-play-integrity-fix-safetynet-fix.4607985/), [MagiskHide Props Config](https://forum.xda-developers.com/t/module-magiskhide-props-config-safetynet-prop-edits-and-more-v5-4-0.3789228/) or [Universal SafetyNet Fix](https://forum.xda-developers.com/t/magisk-module-universal-safetynet-fix-1-1-0.4217823/), renaming your TWRP folder on storage to something else, and using the option in Magisk Settings to Hide the Magisk app.
{% endhint %}

## Search your device's exact model on XDA Developers Forums

Again, you cannot just follow any tutorial or guide for rooting your phone. The best place to find information for your device would be on [XDA Developers Forums](https://xdaforums.com/all-forums-by-manufacturer).
