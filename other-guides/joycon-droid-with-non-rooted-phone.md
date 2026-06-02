---
description: Use a spare rooted Android device to help a non-rooted one connect.
---

# JoyCon Droid With Non-Rooted Phone

#### This is a method to get a non-rooted Android device connected with the Switch. You will need a second spare device that _is_ rooted or have a friend with one assist you. This is not guaranteed to work!

{% hint style="warning" %}
This workaround is a temporary fix since your Android device's Bluetooth MAC address can change or a Switch update may unpair previously connected devices causing you to redo this process. This is not guaranteed to work!
{% endhint %}

### What you need: <a href="#what-you-need" id="what-you-need"></a>

* A [rooted](rooting-with-magisk-and-installing-custom-roms.md) Android device with [Bluetooth HID Profiles support](../other-projects/bluetooth-hid-profile-tester.md) and Magisk.
* A non-rooted Android with Bluetooth HID Profiles support (**must be Samsung if you want to** [**use amiibos**](../guides/using-amiibo.md))

1\) On the rooted Android, follow the [Bluetooth++ guide](../guides/bluetoothpp.md) or [SwitchControllerCOD guide](switchcontroller-cod.md) to change the Device Class to 002508

2\) Find the Bluetooth MAC Address of your non-rooted Android and change the rooted Android's Bluetooth MAC address to the Bluetooth MAC address of the non-rooted Android. Instructions from step 3 [here](alternative-to-bluetooth++.md). (Instead of a real controller, you will change the MAC address to the non-rooted phone.)

3\) Now connect your rooted phone that has copied your non-rooted phone's Bluetooth MAC address to your Switch using JoyCon Droid and make sure it's paired.

4\) Your Switch should remember that Bluetooth MAC Address so you can disconnect the rooted Android now.

5\) Try to connect with your non-rooted Android.



### Note: The rooted Android does not necessarily need Magisk. It just has to be [rooted](rooting-with-magisk-and-installing-custom-roms.md) in general so you are able to change your device class, enable Bluetooth HID Profiles manually if needed, or change Bluetooth MAC address manually. Magisk is usually easier since you can just flash a module and remove/disable the modules if something goes wrong.



## Linux Alternative

If you have access to a computer with Bluetooth, you can either run Linux natively or use a virtual machine with another software (unrelated to JoyCon Droid) called [joycontrol](https://github.com/Poohl/joycontrol). With joycontrol, you can use your PC or Linux machine, such as a raspberry pi, as a controller for the Switch and even use amiibos.&#x20;

You can simply use joycontrol if it works for you but it can also be used as another method of getting your Android device with JoyCon Droid to connect to the Switch if it is not rooted or if you have issues with Bluetooth++ or the MAC address workaround. You would just need to change your Linux device's Bluetooth MAC address to your phone's Bluetooth MAC address and have a successful pair to the Switch using joycontrol before trying to use JoyCon Droid this way.&#x20;

Your Android device still needs to have [Bluetooth HID Profiles](../other-projects/bluetooth-hid-profile-tester.md) support to work as a controller so please click the link to test it first. If you want to [use amiibos](../guides/using-amiibo.md) then it also still needs to be a Samsung device OR another device with a custom ROM based on LineageOS 16+/AOSP built after September 2020 because of the requirement of HID DEV MTU SIZE of 512 bytes.&#x20;

[joycontrol](https://github.com/Poohl/joycontrol)

[Bluetooth adapter compatibility for joycontrol and changing BT MAC Address on Linux](https://github.com/Poohl/joycontrol/issues/4)

[Virtual Machine PDF Guide](https://cdn.discordapp.com/attachments/667167594687496206/983036938544103444/Tutorial.pdf) (Unofficial PDF guide created by a community member on Discord)
