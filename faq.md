---
description: Frequently Asked Questions and important information for using JoyCon Droid.
---

# FAQ

## **Why do I need Android 9 or higher?** <a href="#why-do-i-need-android-9-or-higher" id="why-do-i-need-android-9-or-higher"></a>

Bluetooth HID Profiles were introduced in Android 9 which allow your device to function as a gamepad, mouse, keyboard, etc. You cannot do this on lower Android versions. Use the [Tester app](other-projects/bluetooth-hid-profile-tester.md) to check if you have it. **Android 13** and higher must also install the [SwitchControllerCOD](other-guides/joy-con-droid-companion.md) Magisk module instead of Bluetooth++ due to significant changes to Bluetooth. If using Android 13+, make sure to download the newest version of the app, at least 1.0.91.

## Why do I need [root](other-guides/rooting-with-magisk-and-installing-custom-roms.md)? <a href="#why-do-i-need-root" id="why-do-i-need-root"></a>

Switch firmware version 12.0.0 and up has changed the functionality behind controller connection and input. It now has a Bluetooth Device Class check for initial pairing requests which checks if your device is a Gamepad or others. If your device is on Android 9 to Android 12, it must be rooted with Magisk to use the [Bluetooth++ module](guides/bluetoothpp.md) and change your device class to `002508` **or** to change your device’s Bluetooth MAC address to a real controller you have already paired with the Switch. [Click here for how to use Bluetooth++](guides/bluetoothpp.md). Root is also needed if you want to try to [enabling support for Bluetooth HID Profiles](other-projects/bluetooth-hid-profile-tester.md#if-the-tester-app-fails).

If your device is on Android 13 or higher, you must use the [SwitchControllerCOD](other-guides/joy-con-droid-companion.md) Magisk module instead.

Magisk is not necessarily required, however. You can be rooted with an alternative like SuperSU as well and would just have to manually install or edit your files by accessing them with root privileges. Magisk is recommended and easier since you can simply install or remove the module. KernelSU is another option which can install Magisk modules.

**The JoyCon Droid app itself does not need root, but the workarounds needed to get paired with the Switch need root.**

## How can I [root](other-guides/rooting-with-magisk-and-installing-custom-roms.md) my Android or install custom ROMs? <a href="#how-can-i-root-my-android-or-install-custom-roms" id="how-can-i-root-my-android-or-install-custom-roms"></a>

Every device is different and may use a different set of instructions with unique files to gain root access. Some phones have a difficult process to unlock the bootloader which is needed to flash a custom recovery and install custom ROMs or root with Magisk. Some phones might also be impossible to unlock or root. The best thing to do is search your device’s exact model on [XDA Developers Forums](https://forum.xda-developers.com/). **Please also** [**read the information here**](other-guides/rooting-with-magisk-and-installing-custom-roms.md) **if you are new to rooting Android.**

{% hint style="warning" %}
This process requires a PC, erases everything on your phone, may cause issues with certain apps due to [Play Integrity](https://xdaforums.com/t/info-play-integrity-api-replacement-for-safetynet.4479337/), [SafetyNet Attestation](https://developer.android.com/training/safetynet/attestation), etc. Make sure to backup important data before proceeding or use a spare Android device. You can end up with a non-functioning brick if you do not follow the instructions for your specific Android device carefully.
{% endhint %}

## The Tester app failed. Can I still enable support for Bluetooth HID Profiles?

Yes, you can try using the [Bluetooth HID Enabler Magisk Module](other-projects/bluetooth-hid-profile-tester.md#if-the-tester-app-fails). This still requires Android 9+ and a rooted phone with Magisk to install modules. This module can help for devices that usually have it disabled such as OnePlus, Motorola, Huawei, LG, Sony, and Xiaomi. Restart your device after installing and enabling the module, then try the Tester app again.

## JoyCon Droid from the Play Store?

JoyCon Droid has been removed from the Google Play Store. Anything using the same name is a fake or has uploaded code without permission and should be avoided unless linked here or on Discord. You can install the APK from [GitHub here.](https://github.com/TeamJCD/JoyConDroid/releases/latest)

{% embed url="https://github.com/TeamJCD/JoyConDroid/releases/latest" %}

## Is it safe to change my Android's Bluetooth Device Class? <a href="#is-it-safe-to-change-my-androids-bluetooth-device-class" id="is-it-safe-to-change-my-androids-bluetooth-device-class"></a>

There is always some risk to rooting your phone and modifying system settings. Bluetooth++ will save your default Device Class so you can always reselect it after you're done playing with your Switch. It is however encouraged to make backups before doing any of this as a good practice of safety.

## Why does my phone keep disconnecting from the Switch? <a href="#why-does-my-phone-keep-disconnecting-from-the-switch" id="why-does-my-phone-keep-disconnecting-from-the-switch"></a>

Disconnect any other Bluetooth devices that are connected to your phone such as headphones, speakers, smartwatches, etc. Try the [connection workaround](guides/connecting-to-your-switch.md#if-joycon-droid-disconnects-from-the-switch-after-leaving-the-change-grip-order-screen) and make sure to [save your Android's Bluetooth MAC address in JoyCon Droid Settings](guides/connecting-to-your-switch.md#id-1-save-your-androids-bluetooth-mac-address-in-joycon-droid). Retry connection by Disconnecting Controller using the status bar notifcation on Android and leaving the Change Grip/Order screen **or** Restart both your Switch and Android. \
\
To yield the best results when trying to connect during disconnecting issues, turn off Bluetooth on your Android device and let the JoyCon Droid controller turn it back on for you. This should usually then ask, "Joy-Con Droid wants to make your phone visible to other Bluetooth devices for 60 seconds". Allow it, then try the [connection workaround](guides/connecting-to-your-switch.md#if-joycon-droid-disconnects-from-the-switch-after-leaving-the-change-grip-order-screen). Doing this process with a [real detached Left Joy-Con](guides/connecting-to-your-switch.md#real-left-joy-con-right-joycon-for-amiibo) (connected wirelessly) and Right JoyCon from the app (or even Pro Controller) will make the connection more stable in most cases.

It's also possible you have a Samsung Galaxy A50/A51 which is known to give problems with connecting after a Samsung system update.

If you're using Android 13, you'll need to make sure you're using the latest JoyCon Droid version and use [SwitchController COD](other-guides/joy-con-droid-companion.md) instead if Bluetooth++ doesn't work.

#### Please be aware that the app can be unstable and it can take you multiple tries to get connected properly.  <a href="#please-be-aware-that-the-app-can-be-unstable-and-it-can-take-you-multiple-tries-to-get-connected-pro" id="please-be-aware-that-the-app-can-be-unstable-and-it-can-take-you-multiple-tries-to-get-connected-pro"></a>

## After connecting JoyCon Droid successfully, the Switch keeps asking to do a controller update?

If your Switch [asks you to do a controller update](guides/connecting-to-your-switch.md#if-your-switch-asks-you-to-update-controller-dont-do-it-press-later) for a controller from JoyCon Droid, DO NOT do it. It will get stuck. Press **Later** to skip that popup. If you accidentally pressed Update, simply disconnect the controller by using the Status Bar notification on your phone or turn off Bluetooth.

## The app disconnects when I try to launch a game

Certain games may cause JoyCon Droid to disconnect when they are started as it brings up the same screen as the Change Grip/Order screen in-game. This can cause the app to disconnect frequently and make it difficult to get reconnected to enter and play the game. If this happens to you, turning off Bluetooth on your Android device and then trying to connect may help, repeat if necessary.&#x20;

Using a [real detached Left Joy-Con](guides/connecting-to-your-switch.md#real-left-joy-con-right-joycon-for-amiibo) with a Right JoyCon from the app might be a lot more stable on that screen than a Pro Controller by itself from the app. It may also help the Pro Controller from the app as long as a real controller like a Joy-Con is connected.

Another thing that may help in certain games is to enable Airplane Mode on your Switch, then go into the Switch settings, Airplane Mode section, and then you can turn on only Bluetooth to then see if this helps with connecting.

## What is needed to use amiibos?

`Bluetooth HID_DEV_MTU_SIZE 512`. _Most_ Samsung devices will have this already. LineageOS 16.0 or higher based custom ROMs built after 7th of September 2020 are likely to have this. Make sure to Enable NFC in JoyCon Droid Settings. You can select and change an amiibo `.bin` file in Settings where it says NFC Binary Path. [Go here for more information on using amiibo](guides/using-amiibo.md). \[The Patch introduced on 7th of September 2020 is only for the AOSP Bluetooth Stack. If an Android device uses the Qualcomm Bluetooth Stack, HID\_DEV\_MTU\_SIZE is still set to 64.**]**

## My phone doesn't have NFC. Can I use amiibos? <a href="#my-phone-doesnt-have-nfc-can-i-use-amiibos" id="my-phone-doesnt-have-nfc-can-i-use-amiibos"></a>

Yes. It does not matter if your phone has NFC or not. amiibos are being sent through Bluetooth.

## Where can I get amiibos from? <a href="#where-can-i-get-amiibos-from" id="where-can-i-get-amiibos-from"></a>

Since amiibos are copyrighted content, **JoyCon Droid cannot help you obtain amiibo .bin files for legal reasons**. It is assumed that you are using personal dumped copies of your own amiibos such as from [Tagmo](https://github.com/HiddenRamblings/TagMo).

## amiibos aren't working for me?

Once again, amiibos only work with Samsung devices **or** with a custom ROM such as LineageOS 16.0 or higher, and the custom ROM needs to be built after 2020-07-September because they have a Bluetooth HID\_DEV\_MTU\_SIZE of 512 bytes. If you have this, try other amiibos and [try a combination of a REAL Left Joy-Con and a Right JoyCon in JoyCon Droid](guides/connecting-to-your-switch.md#real-left-joy-con-right-joycon-for-amiibo) and also try changing the Packet Rate to other values such as 10, 20, 50, 69, 80, 120 pps in JoyCon Droid settings. Please be aware that the app can be unstable and it can take you multiple tries to get connected properly and "scan" amiibos.

## Can I resize the buttons or customize the layout of my controller on JoyCon Droid?

Yes, you can Select and Edit a Custom UI from the menu options _of_ JoyCon Droid. You will also find other custom UI options created by members of the community such _&#x61;_&#x73; Macros and TAS UI here. You must have an Internet connection to access these Custom UI options.

## How do I use a gamepad/controller with JoyCon Droid?

You can connect a gamepad to your phone using USB. You may need a USB OTG adapter. **You can’t connect it through Bluetooth** due to the way JoyCon Droid utilizes the Bluetooth connection to pair with the Switch. To avoid connection issues, you must also disconnect other devices such as wireless speakers, smartwatches, etc. **To Remap Buttons/keys, find `Map Buttons` in the menu options of JoyCon Droid.**

## Can I get banned for using JoyCon Droid?

JoyCon Droid has had millions of downloads from users. No one has ever gotten banned yet. There's currently no way that your Switch can tell the difference between JoyCon Droid and a real Switch controller. Your Switch does not need any CFW or modifcations for this to work. You should be safe, but there could still be some risk such as if you use Macros or Turbo Controller to cheat in online multiplayer games and someone reports you.

## Does this app work with the Switch Lite? <a href="#does-this-app-work-with-the-switch-lite" id="does-this-app-work-with-the-switch-lite"></a>

Yes.<br>

## Is there support for Switch 2?

Yes.

## Is there really no way to use a non-rooted Android? <a href="#is-there-really-no-way-to-use-a-non-rooted-android" id="is-there-really-no-way-to-use-a-non-rooted-android"></a>

If you have a spare [rooted](other-guides/rooting-with-magisk-and-installing-custom-roms.md) Android phone or a friend with one, you can try the method [here](other-guides/joycon-droid-with-non-rooted-phone.md). If the Device Class check is ever removed in future Switch updates, that will probably help again but it's not likely to happen for future Switch firmware updates after 12.0.0. Not guaranteed to work. If your Nintendo Switch is modded, you can also use the [Mission Control sysmodule](https://github.com/ndeadly/MissionControl) and it will bypass the need to root your phone to use JoyCon Droid.

## I've tried everything but fail to get JoyCon Droid to work!

If you've followed this guide carefully, tested different custom ROMs, Android versions, and devices, then you may want to [see this page](joycon-droid-alternatives.md) for alternatives.
