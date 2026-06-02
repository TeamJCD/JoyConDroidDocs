---
description: What your Android needs to be compatible with JoyCon Droid.
---

# Compatibility

### 🔷 Android 9 (Pie) or greater

{% hint style="danger" %}
You may need to try multiple custom ROMs until finding a compatible one.&#x20;
{% endhint %}

### 🔷 Support for Bluetooth HID Profiles. Check with the [Tester app](other-projects/bluetooth-hid-profile-tester.md)

{% hint style="warning" %}
#### Some devices do not have support for Bluetooth HID Profiles by default. A few known manufacturers with this issue are OnePlus, Motorola, Huawei, LG, Sony, and Xiaomi. You can still try installing the **Bluetooth HID Enabler - Magisk Module** **for those devices if the Tester app fails.**
{% endhint %}

### 🔷 Root with Magisk to change Bluetooth Device Class with the Bluetooth++ or SwitchControllerCOD module

The guide for that can be [found here](guides/bluetoothpp.md). Alternatively, you can [use root to change your Android's Bluetooth MAC address](other-guides/alternative-to-bluetooth++.md) to a real JoyCon that you have already paired with the Switch. Find information about [rooting and flashing custom ROMs to your phone here](other-guides/rooting-with-magisk-and-installing-custom-roms.md). KernelSU can also install Magisk modules.\
**The JoyCon Droid app itself does not need root, but the workarounds to get paired with the Switch need root.**

### 🔶 Samsung device or [custom ROM](other-guides/rooting-with-magisk-and-installing-custom-roms.md) with Bluetooth HID\_DEV\_MTU\_SIZE 512 (to use [amiibos](guides/using-amiibo.md))

{% hint style="info" %}
#### LineageOS 16.0 or higher based custom ROMs built after 7th of September 2020 are likely to have Bluetooth HID\_DEV\_MTU\_SIZE 512. There is not a way to view this on your device yet. You would have to look at your custom ROM sources. [For example.](https://github.com/crdroidandroid/android_system_bt/blob/15ef283954c79c903e393945d0bf7f2f94b8761c/internal_include/bt_target.h) \[The Patch introduced on 7th of September 2020 is only for the AOSP Bluetooth Stack. If an Android device uses the Qualcomm Bluetooth Stack, HID\_DEV\_MTU\_SIZE is still set to 64.] <a href="#lineageos-16-0-or-higher-based-custom-roms-built-after-7th-of-september-2020-are-likely-to-have-blue" id="lineageos-16-0-or-higher-based-custom-roms-built-after-7th-of-september-2020-are-likely-to-have-blue"></a>
{% endhint %}

{% hint style="danger" %}
Some devices known to have issues connecting to the Switch:

**Samsung Galaxy A50/A51, Chinese Android ROMs**

A custom ROM or different software version is likely to help.
{% endhint %}

{% hint style="danger" %}
Bluetooth++ does not work with devices using the QTI Bluetooth stack. [More information can be found here.](https://github.com/TeamJCD/BluetoothPlusPlus/issues/3)
{% endhint %}
