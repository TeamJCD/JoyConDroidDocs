---
description: >-
  Magisk module to change Bluetooth Device Class on rooted Android devices for
  compatibility with JoyCon Droid.
---

# Joy-Con Droid Companion

[Joy-Con Droid Companion](https://github.com/TeamJCD/JoyConDroidCompanion) is a new Magisk module created by [dtrunk90](https://github.com/dtrunk90/) intended for rooted Android devices.

{% hint style="danger" %}
Currently, this only supports 64-bit devices. Please see [instructions for Bluetooth++](../guides/bluetoothpp.md) or SwitchControllerCOD instead if you have an older device.
{% endhint %}

## Installation

{% hint style="warning" %}
If you're using Android 13 and have used Bluetooth++ to change your device class to 002508, please select the Default device class (usually 5a020c) in the Bluetooth++ app **before** removing it from Magisk. Otherwise it may remain on 002508 and persist on reboots, which may invalidate test reports for whether the Magisk module actually works or not!
{% endhint %}

1. Make sure your device is running Android 13 or higher and [supports Bluetooth HID Profiles](../other-projects/bluetooth-hid-profile-tester.md).
2. Uninstall the [Bluetooth++](../guides/bluetoothpp.md) or SwitchControllerCOD Magisk module if you have it.
3. Download JoyConDroidCompanion-X.X.X.zip from [GitHub here](https://github.com/TeamJCD/JoyConDroidCompanion/releases/latest).
4. Open Magisk, tap the Modules section, and then tap Install from storage.
5. Select the JoyConDroidCompanion zip file.
6. Tap OK on the Install Confirmation.
7. Tap Reboot when done installing.
8. You can proceed to [using JoyCon Droid](../guides/connecting-to-your-switch.md)! Make sure you have the latest version of JoyCon Droid.

<div><figure><img src="../.gitbook/assets/SCCOD GitHub Releases (1).png" alt="" width="188"><figcaption></figcaption></figure> <figure><img src="../.gitbook/assets/Magisk modules (1).png" alt="" width="188"><figcaption></figcaption></figure> <figure><img src="../.gitbook/assets/install from storage (1).png" alt="" width="188"><figcaption></figcaption></figure> <figure><img src="../.gitbook/assets/SwitchControllerCOD ZIP (1).png" alt="" width="188"><figcaption></figcaption></figure> <figure><img src="../.gitbook/assets/install confirmation (1).png" alt="" width="188"><figcaption></figcaption></figure> <figure><img src="../.gitbook/assets/Reboot (1).png" alt="" width="188"><figcaption></figcaption></figure></div>

## Doesn't work?

If JoyCon Droid still does not connect at all, remove the module and try [Bluetooth++](../guides/bluetoothpp.md) instead. JoyConDroidCompanion does not support legacy 32 bit devices at this time and needs testing.

## Uninstall/Disable

Please note that Joy-Con Droid Companion does not add an application to your device like Bluetooth++ does. When installed and enabled, it simply changes your Bluetooth device class in order for the Switch to accept pairing as it recognizes your phone as a controller.&#x20;

You can disable the module in Magisk and then reboot to revert the changes OR just remove the module and reboot.
