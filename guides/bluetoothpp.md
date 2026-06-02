---
description: >-
  How to install the Bluetooth++ Magisk module and change your Device Class to a
  Gamepad for the Switch to accept pairing connection after firmware update
  12.0.0.
---

# Installing Bluetooth++ and Changing Device Class

Before proceeding, make sure your Android phone is [capable](../compatibility.md) to use JoyCon Droid first. You must also be able to succeed when using the [Bluetooth HID Profile Tester app](../other-projects/bluetooth-hid-profile-tester.md).

{% hint style="danger" %}
## ROOT WITH MAGISK IS REQUIRED

#### Find out what this means by [clicking here](../other-guides/rooting-with-magisk-and-installing-custom-roms.md). <a href="#find-out-what-this-means-by-clicking-here" id="find-out-what-this-means-by-clicking-here"></a>

#### ⚠️ Bluetooth++ is not compatible with many newer Android devices using the Qualcomm (QTI) Bluetooth stack because it cannot change the Device Class yet. This is only possible with the AOSP Bluetooth stack. If you have a device that doesn't work with Bluetooth++, try switching to a different custom ROM such as LineageOS (Some devices may work if downgrading to Android 9 or 10), or try the [MAC address trick](../other-guides/alternative-to-bluetooth++.md) which will let your phone connect to the Switch after changing the phone's MAC address, using root, to appear as a real controller that has been connected to your Switch already. <a href="#xiaomi-miui-is-not-supported-bluetooth-is-not-compatible-with-it-because-miui-is-a-heavily-modified" id="xiaomi-miui-is-not-supported-bluetooth-is-not-compatible-with-it-because-miui-is-a-heavily-modified"></a>
{% endhint %}

{% hint style="warning" %}
## Bluetooth++ only supports Android 9 to Android 12.

If you are using Android 13 or higher, DO NOT install Bluetooth++. Please see instructions for the [SwitchControllerCOD](../other-guides/joy-con-droid-companion.md) Magisk module instead. Certain devices/ROMs on Android 13 may still be able to use Bluetooth++. Test both (not at the same time) if you have issues connecting on Android 13.
{% endhint %}

![The Magisk app will show you if Magisk is installed](<../.gitbook/assets/image (9).png>)

#### If Magisk shows N/A near Installed, then you do not have Magisk installed yet.

## 1. Download the latest release of [BluetoothPlusPlus-x.x.zip](https://github.com/TeamJCD/BluetoothPlusPlus/releases/latest) <a href="#id-1-download-the-latest-release-of-bluetoothplusplus-x-x-zip" id="id-1-download-the-latest-release-of-bluetoothplusplus-x-x-zip"></a>

## 2. Now go to the Modules tab of Magisk and tap Install from storage at the top. Then select BluetoothPlusPlus-x.x.zip from the file chooser.

![](../.gitbook/assets/Screenshot_20210821-183033894_1.jpg)

![](<../.gitbook/assets/image (10).png>)

## 3. Reboot your Android after installing the module.

![](<../.gitbook/assets/image (46).png>)

## 4. After rebooting, you will find a new app called Bluetooth++ in your app drawer. Open this app.

![](<../.gitbook/assets/image (8).png>)

## 5. If your Bluetooth isn't enabled when opening the app, it will ask you to turn it on. Tap Allow.

![](<../.gitbook/assets/image (34).png>)

## 6. The app will show you your phone's default Device Class. Yours may be different from the one pictured. &#x20;

![](<../.gitbook/assets/image (48).png>)

## 7. Tap the (+) icon in the top right of the image above to create a new Device Class. <a href="#id-7-tap-the-icon-in-the-top-right-of-the-image-above-to-create-a-new-device-class" id="id-7-tap-the-icon-in-the-top-right-of-the-image-above-to-create-a-new-device-class"></a>

## 8. You must now choose a name and enter the correct Device Class. Tap on Name and Device Class to enter text. The name can be anything such as "Switch Controller" and the Device Class must be 002508 <a href="#id-8-you-must-now-choose-a-name-and-enter-the-correct-device-class-tap-on-name-and-device-class-to-ente" id="id-8-you-must-now-choose-a-name-and-enter-the-correct-device-class-tap-on-name-and-device-class-to-ente"></a>

![](<../.gitbook/assets/image (47).png>)

## 9. Make sure the Device Class is entered correctly. 002508 is the Device Class for a Gamepad. Then tap the 3-dot symbol (menu) button on the top right to Save.

![](<../.gitbook/assets/image (4).png>)

## 10. You'll now see the new Device Class in the app. Select this new Device Class anytime before using JoyCon Droid and it should help you connect to the Switch if everything is working as expected.

![](<../.gitbook/assets/image (23).png>)



* You should switch to your Default device class when not using JoyCon Droid to avoid potential connectivity issues with your other devices.



* If you're not rooted with Magisk for some reason such as SuperSU or just want an alternative to Bluetooth++, you can try to install the files manually or you can try a different method. [Check here for how to change your Bluetooth MAC address to a real Switch controller that was connected to the Switch before](../other-guides/alternative-to-bluetooth++.md).

### Removing the module: <a href="#removing-the-module" id="removing-the-module"></a>

If you need to remove the module, first select your Default device class again. After that, you can simply disable the module or remove the module in Magisk and then reboot your device. If you somehow get stuck in a bootloop, you will need to remove modules through your custom recovery or safe mode. [Remove Magisk modules in an emergency](https://topjohnwu.github.io/Magisk/faq.html) or completely uninstall Magisk by renaming Magisk APK to uninstall.zip and flash the zip in recovery like usual.
