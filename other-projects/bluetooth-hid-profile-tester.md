---
description: >-
  Test if you have support for Bluetooth HID Profiles on your Android 9 or
  higher device.
---

# Bluetooth HID Profile Tester

{% embed url="https://play.google.com/store/apps/details?id=com.rdapps.bluetoothhidtester" %}
Download Bluetooth HID Profile Tester from Google Play
{% endembed %}

### Turn on Bluetooth and test if your Android 9 or greater device has support for Bluetooth HID Profiles. <a href="#turn-on-bluetooth-and-test-if-your-android-9-or-greater-device-has-support-for-bluetooth-hid-profile" id="turn-on-bluetooth-and-test-if-your-android-9-or-greater-device-has-support-for-bluetooth-hid-profile"></a>

### The following image will be seen on your device if the test is successful: <a href="#the-following-image-will-be-seen-on-your-device-if-the-test-is-successful" id="the-following-image-will-be-seen-on-your-device-if-the-test-is-successful"></a>

![A successful test is usually quick.](<../.gitbook/assets/image (24).png>)

{% hint style="info" %}
Please note that a successful test is not enough to use JoyCon Droid. Your Android device still needs to be [rooted](../other-guides/rooting-with-magisk-and-installing-custom-roms.md) in order to change its Bluetooth Device Class. If the test is successful and your device is rooted, proceed to changing the device class with [Bluetooth++](../guides/bluetoothpp.md) (Android 9-13) or [SwitchController COD](../other-guides/joy-con-droid-companion.md) (Android 13+).
{% endhint %}

### The following image will be seen on your device if the test fails: <a href="#the-following-image-will-be-seen-on-your-device-if-the-test-fails" id="the-following-image-will-be-seen-on-your-device-if-the-test-fails"></a>

![A failed test usually takes longer to complete.](<../.gitbook/assets/image (43).png>)

## If the Tester app fails?

#### If the tester app fails, it means your device firmware does not have Bluetooth HID Profiles enabled or implemented, and is unable to function as a gamepad controller or other Human Interface Devices.  <a href="#if-the-tester-app-fails-it-means-your-device-firmware-does-not-have-bluetooth-hid-profiles-enabled-o" id="if-the-tester-app-fails-it-means-your-device-firmware-does-not-have-bluetooth-hid-profiles-enabled-o"></a>

{% hint style="info" %}
#### You can still try to enable Bluetooth HID Profiles if your Android device is [rooted](../other-guides/rooting-with-magisk-and-installing-custom-roms.md) with Magisk and is ≥ Android 9 with a Magisk module.
{% endhint %}

#### In Magisk, install blefinal.zip from GitHub [here.](https://github.com/LoreBadTime/Bluetooth-HID-Enabler/releases/latest)

#### Reboot after installing and retry the Tester app! <a href="#reboot-after-installing-and-retry-the-tester-app" id="reboot-after-installing-and-retry-the-tester-app"></a>



If that fails, try the old version:&#x20;

In Magisk, install magisk-bluetoothhidenabler-v2.zip from GitHub [here.](https://github.com/ysc3839/magisk-bluetoothhidenabler/releases/latest)

### Alternatively, you can just use root to manually edit the required files in your device. Check this [video](https://www.youtube.com/watch?v=yXtbVBTZVXA) for how to do that. The Magisk module would of course be easier than this though. The location of your Bluetooth file may vary from the one in the video. <a href="#alternatively-you-can-just-use-root-to-manually-edit-the-required-files-in-your-device-check-this-vi" id="alternatively-you-can-just-use-root-to-manually-edit-the-required-files-in-your-device-check-this-vi"></a>
