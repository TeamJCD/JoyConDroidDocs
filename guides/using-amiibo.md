---
description: >-
  Using amiibo .bin files with JoyCon Droid. Not all phones can use amiibo.
  Check below for either the Samsung or custom ROM requirements.
---

# Using amiibo

{% hint style="danger" %}
You won't get help for finding and downloading amiibos. You must use your own amiibo `.bin` backups. [The FAQ explains this.](../faq.md#where-can-i-get-amiibos-from)
{% endhint %}

### Only Samsung & Custom ROMs (other phones) can use amiibo! <a href="#samsung-vs-custom-roms-more-phones" id="samsung-vs-custom-roms-more-phones"></a>

{% hint style="info" %}
## **Samsung**

Samsung is the only known smartphone manufacturer that usually has a large enough Bluetooth HID\_DEV\_MTU\_SIZE found in the stock system firmware. Most of the time you do not need to flash a custom ROM if you have a Samsung device. A custom ROM on Samsung devices might only be necessary if you have an older device and need to upgrade to Android 9 (P) or greater.
{% endhint %}

{% hint style="info" %}
## **Custom ROMs For Other Phones**

With [custom ROM](../other-guides/rooting-with-magisk-and-installing-custom-roms.md)s, you can use amiibos on almost all other kinds of Android devices. The ROM you install needs to have `HID_DEV_MTU_SIZE 512`&#x20;

Most ROMs that are LineageOS 16.0 based and higher built after 2020-07-September are highly likely to have this and be capable of using amiibo. It's not yet possible to check this on your device besides looking at your ROM source. [For example.](https://github.com/crdroidandroid/android_system_bt/blob/15ef283954c79c903e393945d0bf7f2f94b8761c/internal_include/bt_target.h) \[The Patch introduced on 7th of September 2020 is only for the AOSP Bluetooth Stack. If an Android device uses the Qualcomm Bluetooth Stack, HID\_DEV\_MTU\_SIZE is still set to 64.]

#### Custom ROMs that have `HID_DEV_MTU_SIZE 512`  <a href="#custom-roms-that-have-hid_dev_mtu_size-512" id="custom-roms-that-have-hid_dev_mtu_size-512"></a>

* LineageOS 16.0 and higher (built after 2020-07 September)
* Evolution X
* crDroid
* Many more if based on LineageOS and built recently after 2020 07 September

You can find your ROM's Build date by checking the date on the ROM you flashed or going to your phone's **Settings** app → **About phone** (open **System** first on some phones) → **Android version** (open **Status** first on some phones) → **Build date**
{% endhint %}

{% hint style="warning" %}
#### If you're not able to get amiibos working, try [using a **real Left Joy-Con** with a **Right JoyCon (in JoyCon Droid)**](connecting-to-your-switch.md#real-left-joy-con-right-joycon-for-amiibo) and also try **changing the** Packet Rate in JoyCon Droid Settings. <a href="#if-youre-not-able-to-get-amiibos-working-you-need-to-try-using-a-real-left-joy-con-with-a-right-joyc" id="if-youre-not-able-to-get-amiibos-working-you-need-to-try-using-a-real-left-joy-con-with-a-right-joyc"></a>

#### Please be aware that the app can be unstable and it can take you multiple tries to get connected properly and "scan" amiibos. <a href="#please-be-aware-that-the-app-can-be-unstable-and-it-can-take-you-multiple-tries-to-get-connected-pro" id="please-be-aware-that-the-app-can-be-unstable-and-it-can-take-you-multiple-tries-to-get-connected-pro"></a>
{% endhint %}

## **How to use amiibo:** <a href="#how-to-use-amiibo" id="how-to-use-amiibo"></a>

### You first need to enable NFC in JoyCon Droid Settings before you can use amiibo <a href="#you-first-need-to-enable-nfc-in-joycon-droid-settings-before-you-can-use-amiibo" id="you-first-need-to-enable-nfc-in-joycon-droid-settings-before-you-can-use-amiibo"></a>

#### Tap the menu icon in JoyCon Droid

![](<../.gitbook/assets/image (36).png>)

#### Tap Settings

![](<../.gitbook/assets/image (11).png>)

#### Turn on Enable NFC

![](<../.gitbook/assets/image (18).png>)

#### You will get a warning if you're using a non-Samsung device or custom ROM and also letting you know that this is experimental and might not work. Tap Continue if you believe to have a compatible Samsung or a phone with a [custom ROM](../other-guides/rooting-with-magisk-and-installing-custom-roms.md) that has Bluetooth HID\_DEV\_MTU\_SIZE 512. <a href="#you-will-get-a-warning-if-youre-using-a-non-samsung-device-or-custom-rom-and-also-letting-you-know-t" id="you-will-get-a-warning-if-youre-using-a-non-samsung-device-or-custom-rom-and-also-letting-you-know-t"></a>

![Tap Continue](<../.gitbook/assets/image (41).png>)

![Tap Continue](<../.gitbook/assets/image (16).png>)

#### Now tap Select to find an amiibo .bin file from your device. Put all of your amiibos in a folder so you can find them easily. <a href="#now-tap-select-to-find-an-amiibo-bin-file-from-your-device-put-all-of-your-amiibos-in-a-folder-so-yo" id="now-tap-select-to-find-an-amiibo-bin-file-from-your-device-put-all-of-your-amiibos-in-a-folder-so-yo"></a>

![Tap Select](<../.gitbook/assets/image (28).png>)

![Find and select an amiibo .bin that you want to use.](<../.gitbook/assets/image (20).png>)

![You will see what amiibo you currently have Selected.](<../.gitbook/assets/image (2).png>)

### The .bin you chose can be seen under NFC Binary Path. You can now try to connect JoyCon Droid to your Switch and use it in your game.

#### To select a different amiibo, change it the same way above in NFC Binary Path.

{% hint style="info" %}
## If you're having issues getting an amiibo to work, try [using a combination of a REAL Left JoyCon and a Right JoyCon from JoyCon Droid](connecting-to-your-switch.md#real-left-joy-con-right-joycon-for-amiibo). <a href="#if-youre-having-issues-getting-an-amiibo-to-work-try-using-a-combination-of-a-real-left-joycon-and-a" id="if-youre-having-issues-getting-an-amiibo-to-work-try-using-a-combination-of-a-real-left-joycon-and-a"></a>

## You may also need to change the Packet Rate for better success to values such as 10, 20, 50, 69, 80, 120 pps. <a href="#if-youre-having-issues-getting-an-amiibo-to-work-try-using-a-combination-of-a-real-left-joycon-and-a" id="if-youre-having-issues-getting-an-amiibo-to-work-try-using-a-combination-of-a-real-left-joycon-and-a"></a>
{% endhint %}

![](<../.gitbook/assets/image (49).png>)

{% hint style="info" %}
### Make sure you chose a `.bin` file. You could have a corrupted .bin such as from an incomplete download so try redownloading it. <a href="#make-sure-you-chose-a-bin-file-you-could-have-a-corrupted-bin-such-as-from-an-incomplete-download-so" id="make-sure-you-chose-a-bin-file-you-could-have-a-corrupted-bin-such-as-from-an-incomplete-download-so"></a>

### Try out different amiibos. <a href="#make-sure-you-chose-a-bin-file-you-could-have-a-corrupted-bin-such-as-from-an-incomplete-download-so" id="make-sure-you-chose-a-bin-file-you-could-have-a-corrupted-bin-such-as-from-an-incomplete-download-so"></a>

### Change the Packet Rate.

### Make sure you're using a Samsung phone OR a custom ROM that was built after 2020-07 September and has Bluetooth HID\_DEV\_MTU\_SIZE 512 \[The Patch introduced on 7th of September 2020 is only for the AOSP Bluetooth Stack. If an Android device uses the Qualcomm Bluetooth Stack, HID\_DEV\_MTU\_SIZE is still set to 64.] <a href="#make-sure-you-chose-a-bin-file-you-could-have-a-corrupted-bin-such-as-from-an-incomplete-download-so" id="make-sure-you-chose-a-bin-file-you-could-have-a-corrupted-bin-such-as-from-an-incomplete-download-so"></a>
{% endhint %}
