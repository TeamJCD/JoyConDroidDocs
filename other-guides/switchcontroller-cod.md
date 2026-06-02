---
description: >-
  Magisk module to change Bluetooth Device Class on Android 13 and higher
  devices for compatibility with JoyCon Droid.
---

# SwitchController COD

[SwitchController COD](https://github.com/TeamJCD/SwitchControllerCOD) is a new Magisk module created by [dtrunk90](https://github.com/dtrunk90/) intended for rooted devices running Android 13 or greater. Since Android 13 and 14, significant changes were done to Bluetooth within the system. This module should help these devices connect to the Switch again.&#x20;

{% hint style="danger" %}
SwitchController COD is only for devices running Android 13 and higher. If your device runs Android 9 to Android 12, do not install this. Please see [instructions for Bluetooth++](../guides/bluetoothpp.md) instead!
{% endhint %}

## Installation

{% hint style="warning" %}
If you're using Android 13 and have used Bluetooth++ to change your device class to 002508, please select the Default device class (usually 5a020c) in the Bluetooth++ app **before** removing it from Magisk. Otherwise it'll remain on 002508 and persist on reboots, which may invalidate test reports for whether SwitchController COD actually works or not!
{% endhint %}

1. Make sure your device is running Android 13 or higher and [supports Bluetooth HID Profiles](../other-projects/bluetooth-hid-profile-tester.md).
2. Uninstall the [Bluetooth++](../guides/bluetoothpp.md) Magisk module if you have it.
3. Download SwitchControllerCOD-X.X.X.zip from [GitHub here](https://github.com/TeamJCD/SwitchControllerCOD/releases/latest).
4. Open Magisk, tap the Modules section, and then tap Install from storage.
5. Select the SwitchControllerCOD zip file.
6. Tap OK on the Install Confirmation.
7. Tap Reboot when done installing.
8. You can proceed to [using JoyCon Droid](../guides/connecting-to-your-switch.md)! Make sure you have the latest version of JoyCon Droid, at least 1.0.91.

<div><figure><img src="../.gitbook/assets/SCCOD GitHub Releases (1).png" alt="" width="188"><figcaption></figcaption></figure> <figure><img src="../.gitbook/assets/Magisk modules (1).png" alt="" width="188"><figcaption></figcaption></figure> <figure><img src="../.gitbook/assets/install from storage (1).png" alt="" width="188"><figcaption></figcaption></figure> <figure><img src="../.gitbook/assets/SwitchControllerCOD ZIP (1).png" alt="" width="188"><figcaption></figcaption></figure> <figure><img src="../.gitbook/assets/install confirmation (1).png" alt="" width="188"><figcaption></figcaption></figure> <figure><img src="../.gitbook/assets/Reboot (1).png" alt="" width="188"><figcaption></figcaption></figure></div>

## Doesn't work?

If you are using Android 13 and JoyCon Droid still does not connect at all, remove SwitchController COD and try [Bluetooth++](../guides/bluetoothpp.md) instead. SwitchController COD might not work with some earlier builds of Android 13.

For Android 14 and up, only SwitchController COD can be used. Please report issues in the #testers-report channel of Discord.

## Uninstall/Disable

Please note that SwitchController COD does not add an application to your device like Bluetooth++ does. When installed and enabled, it simply changes your Bluetooth device class in order for the Switch to accept pairing as it recognizes your phone as a controller.&#x20;

You can simply disable the module in Magisk and then reboot to revert the changes OR just remove the module and reboot.
