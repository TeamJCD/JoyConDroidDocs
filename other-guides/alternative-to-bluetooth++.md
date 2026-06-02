---
description: An alternative root method for connecting to the Switch with JoyCon Droid
---

# Alternative to Bluetooth++

{% hint style="success" %}
#### You don't need to do this if you have already changed your Device Class using the Bluetooth++ Magisk module! You can proceed to [Connecting to your Switch.](../guides/connecting-to-your-switch.md)​ The method on this page is for devices using the Qualcomm (QTI) Bluetooth Stack which does not yet work with Bluetooth++. <a href="#you-dont-need-to-do-this-if-you-have-already-changed-your-device-class-using-the-bluetooth-magisk-mo" id="you-dont-need-to-do-this-if-you-have-already-changed-your-device-class-using-the-bluetooth-magisk-mo"></a>
{% endhint %}

{% hint style="danger" %}
## Requires [root.](rooting-with-magisk-and-installing-custom-roms.md) This method can be risky if you do something wrong in the procedure. It is recommended to try the [Bluetooth++ Magisk module method](../guides/bluetoothpp.md) instead of doing this (only works on devices using the AOSP Bluetooth stack). Make a backup of your phone and bluetooth file before continuing. DO AT YOUR OWN RISK! This is not guaranteed to work. <a href="#requires-root-this-method-is-very-risky-if-you-do-something-wrong-in-the-procedure-it-is-recommended" id="requires-root-this-method-is-very-risky-if-you-do-something-wrong-in-the-procedure-it-is-recommended"></a>
{% endhint %}

1\. Pair a real controller with your Switch like normal. Yes, a real physical JoyCon or Pro Controller that you have.

2\. Find the Bluetooth MAC address of that controller. You can connect the controller to your phone and find the Device's Bluetooth address in the Device details of Bluetooth settings. You can also use [Joy-Con Toolkit](https://gbatemp.net/threads/tool-joy-con-toolkit.478560/) on PC to view your controller's MAC address.

3\. On your Android, you will need to navigate to  `/efs/bluetooth/bt_addr`&#x20;

`/data/vendor/mac_addr/bt.mac` `,` `/data/misc/bluetooth/bdaddr` or `/data/vendor/bluetooth/bdaddr` and **MAKE A BACKUP of this file!** Root privileges will need to be granted when navigating to and modifying this file. \[**The location of the file for editing Bluetooth MAC Address will vary depending on your device.**]

4\. Change your device's MAC address at `/efs/bluetooth/bt_addr`, `/data/vendor/mac_addr/bt.mac` , `/data/vendor/bluetooth/ bdaddr` **or** `/data/misc/bluetooth/bdadd` with the real controller's MAC address.&#x20;

5\. A reboot might be needed after making the changes. You can try to connect JoyCon Droid to the Switch now.&#x20;

Overwrite the file again with the backup you made to restore your original MAC address if you need to.



#### If you're wondering how to access those files, obviously you need to grant [root](rooting-with-magisk-and-installing-custom-roms.md) access first of all. You can find and edit those files numerous ways such as: adb commands, root explorer ([Total Commander](https://play.google.com/store/apps/details?id=com.ghisler.android.TotalCommander) is free with no ads), [Termux](https://termux.com/) (terminal emulator)

#### On devices having `/data/vendor/mac_addr/bt.mac` (which is usually the case on MIUI devices) you'll need a Hex Editor App (can be installed through Play Store) to edit that file. To change to the desired Bluetooth MAC Address (e.g. a1:b2:c3:d4:e5:f6) you have to put a1b2c3d4e5f6 (without colons) using a Hex Editor.



## [Linux Alternative](joycon-droid-with-non-rooted-phone.md#linux-alternative)

[Click here for joycontrol info.](joycon-droid-with-non-rooted-phone.md#linux-alternative)
