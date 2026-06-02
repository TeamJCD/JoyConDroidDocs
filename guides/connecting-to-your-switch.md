---
description: How to connect to your Switch using JoyCon Droid
---

# Connecting to Your Switch

After making sure your device is [compatible](../compatibility.md), it is time to connect to the Switch! For basic gamepad compatibility (not including amiibo), you need to at least have [support for Bluetooth HID Profiles](../other-projects/bluetooth-hid-profile-tester.md) and have already changed your Device Class to `002508`using the [Bluetooth++](bluetoothpp.md) Magisk module **or** by changing your MAC address using root.

[Main Connection Guide](connecting-to-your-switch.md#steps-to-connect)

[Disconnection Problem Fix](connecting-to-your-switch.md#if-joycon-droid-disconnects-from-the-switch-after-leaving-the-change-grip-order-screen)

[amiibo workaround](connecting-to-your-switch.md#real-left-joy-con-right-joycon-for-amiibo)

{% embed url="https://github.com/TeamJCD/JoyConDroid/releases/latest" %}
Latest JoyCon Droid APK Download
{% endembed %}

{% hint style="info" %}
## Important!

When opening JoyCon Droid for the first time, allow the following permissions when requested or else the app won't function correctly:

<img src="../.gitbook/assets/Allow Notifications.png" alt="" data-size="original">

<img src="../.gitbook/assets/Allow Device Discovery and Connections.png" alt="" data-size="original">
{% endhint %}

## **Steps to connect:**  <a href="#steps-to-connect" id="steps-to-connect"></a>

## 1) Save your **Android's** Bluetooth MAC Address in JoyCon Droid.  <a href="#id-1-save-your-androids-bluetooth-mac-address-in-joycon-droid" id="id-1-save-your-androids-bluetooth-mac-address-in-joycon-droid"></a>

#### This step is technically optional. However, it is very necessary for a better and automatic reconnection to the Switch for certain menus and games. The first time you choose a controller in JoyCon Droid, you will be asked for your Android's Bluetooth MAC Address. <a href="#this-step-is-technically-optional-however-it-is-very-necessary-for-a-better-and-automatic-reconnecti" id="this-step-is-technically-optional-however-it-is-very-necessary-for-a-better-and-automatic-reconnecti"></a>

![](<../.gitbook/assets/image (35).png>)

#### If you skip this, you can also find it in JoyCon Droid Settings later:

![](../.gitbook/assets/image.png)

#### First make sure that Bluetooth is turned on:

![Enable Bluetooth before finding your Bluetooth MAC Address.](<../.gitbook/assets/image (3).png>)

#### To find your Android's Bluetooth MAC address, go to the Settings app of your phone and scroll down to **About phone.**

![On some device models, you will first need to open System.](<../.gitbook/assets/image (21).png>)

#### After opening About phone, scroll down to **Bluetooth address.**

![On some devices, you will first need to open Status to see your Bluetooth address.](<../.gitbook/assets/image (29).png>)

#### Now copy and paste or manually enter your Bluetooth address into JoyCon Droid and then tap Set.

![Double check that you have correctly saved your phone's Bluetooth Address in JoyCon Droid Settings.](<../.gitbook/assets/image (5).png>)

## 2) Choose your controller in JoyCon Droid and Allow it to turn on Bluetooth for you if it’s not already on.

![Choose your controller in JoyCon Droid](<../.gitbook/assets/image (6).png>)

![Allow it to turn it on Bluetooth if it's not on yet.](<../.gitbook/assets/image (7).png>)

## 3) Tap Allow when asked to make your phone visible to other Bluetooth devices for 60 seconds

![](<../.gitbook/assets/image (31).png>)

## 4) On your Switch, go to Controllers → Change Grip/Order. <a href="#id-4-on-your-switch-go-to-controllers-change-grip-order" id="id-4-on-your-switch-go-to-controllers-change-grip-order"></a>

![](<../.gitbook/assets/image (26).png>)

![](<../.gitbook/assets/image (33).png>)

![](<../.gitbook/assets/image (19).png>)

## 5) Tap Pair when the Switch pairing request appears.

#### If you don't see this Pair request, tap the sync button once:

![](<../.gitbook/assets/image (45).png>)

![Tap Pair. You don't need to check the box.](<../.gitbook/assets/image (42).png>)

![](<../.gitbook/assets/image (30).png>)

## 6) After Pairing, your controller should appear on the Switch. If you're using a single JoyCon, you'll need to press SL and SR together first.

![](<../.gitbook/assets/image (1).png>)

![](<../.gitbook/assets/image (40).png>)

![](<../.gitbook/assets/image (22).png>)

## 7) Continue and you should now be connected! <a href="#id-7-continue-with-the-right-action-button-and-you-should-now-be-connected" id="id-7-continue-with-the-right-action-button-and-you-should-now-be-connected"></a>

![](<../.gitbook/assets/image (38).png>)

***

## If your Switch asks you to update controller, don't do it! Press Later. <a href="#if-your-switch-asks-you-to-update-controller-dont-do-it-press-later" id="if-your-switch-asks-you-to-update-controller-dont-do-it-press-later"></a>

![If you accidentally pressed Update, just disconnect JoyCon Droid.](<../.gitbook/assets/image (37).png>)

***

## **To disconnect your controller or select a different one, use the notification in the Status Bar or turn off Bluetooth:**

![Use the Status Bar notification to Disconnect.](<../.gitbook/assets/image (25).png>)

***

## **If JoyCon Droid disconnects from the Switch after leaving the Change Grip/Order Screen:** <a href="#if-joycon-droid-disconnects-from-the-switch-after-leaving-the-change-grip-order-screen" id="if-joycon-droid-disconnects-from-the-switch-after-leaving-the-change-grip-order-screen"></a>

![You might have this problem when leaving the Change/Grip Order Screen.](<../.gitbook/assets/image (44).png>)

### You must connect with the following workaround if this is happening: <a href="#you-must-connect-with-the-following-workaround-if-this-is-happening" id="you-must-connect-with-the-following-workaround-if-this-is-happening"></a>

Before continuing, you may need to disconnect your chosen controller by using the status bar notification and leave the Change Grip/Order screen, turn off Bluetooth on your phone **or** restart both your Android and Switch console.

### 1) Follow steps 1 through 4 from [above](connecting-to-your-switch.md#steps-to-connect), don't skip step 1.

### 2) When you get the Pairing Request, WAIT! Don't press Pair yet!

![WAIT! DO NOT press Pair yet!](<../.gitbook/assets/image (39).png>)

## 3) Exit the Change/Grip Order screen using the Back button. You can press the Back button in handheld mode with your finger: <a href="#id-3-exit-the-change-grip-order-screen-using-the-back-button-you-can-press-the-back-button-in-handheld" id="id-3-exit-the-change-grip-order-screen-using-the-back-button-you-can-press-the-back-button-in-handheld"></a>

![](<../.gitbook/assets/image (17).png>)

## 4) Now you can tap Pair on your Android.

![](<../.gitbook/assets/image (15).png>)

## 5) The controller should now be connected on the Controllers screen! You can Close this screen. <a href="#id-5-the-controller-should-now-be-connected-on-the-controllers-screen-you-can-close-this-screen" id="id-5-the-controller-should-now-be-connected-on-the-controllers-screen-you-can-close-this-screen"></a>

![](<../.gitbook/assets/image (14).png>)

***

## Real Left Joy-Con + Right JoyCon for amiibo <a href="#real-left-joy-con-right-joycon-for-amiibo" id="real-left-joy-con-right-joycon-for-amiibo"></a>

Using a combination of a **REAL Left Joy-Con** and a **Right JoyCon from JoyCon Droid** can increase your success of using amiibos. It might also make the connection process more stable in general. You may also need to change the Packet Rate in JoyCon Droid Settings. Different devices will have varying rates of success using packet rates such as 10, 20, 50, 69, 120 pps, etc.

![Try different rates such as 10, 20, 50, 69, 80,120, etc.](<../.gitbook/assets/image (50).png>)

### 1) Make sure you have done steps 1 through 5 from the [top of this page](connecting-to-your-switch.md#steps-to-connect). <a href="#id-1-make-sure-you-have-done-steps-1-through-5-from-the-top-of-this-page" id="id-1-make-sure-you-have-done-steps-1-through-5-from-the-top-of-this-page"></a>

### 2) Pair your REAL Left JoyCon. You might need to first hold down the sync button on the side. <a href="#id-2-pair-your-real-left-joycon-you-might-need-to-first-hold-down-the-sync-button-on-the-side" id="id-2-pair-your-real-left-joycon-you-might-need-to-first-hold-down-the-sync-button-on-the-side"></a>

### 3) If your Left JoyCon and Right JoyCon (from JoyCon Droid) are paired, you should see this: <a href="#id-3-if-your-left-joycon-and-right-joycon-from-joycon-droid-are-paired-you-should-see-this" id="id-3-if-your-left-joycon-and-right-joycon-from-joycon-droid-are-paired-you-should-see-this"></a>

![](<../.gitbook/assets/image (32).png>)

### 4) Now hold L+R together. (L on your REAL Left Joy-Con and R on the _JoyCon Droid_ Right JoyCon and they will combine: <a href="#id-4-now-hold-l-r-together-l-on-your-real-left-joy-con-and-r-on-the-joycon-droid-right-joycon-and-they" id="id-4-now-hold-l-r-together-l-on-your-real-left-joy-con-and-r-on-the-joycon-droid-right-joycon-and-they"></a>

![](<../.gitbook/assets/image (12).png>)

### 5) Now they are connected and paired:

![](<../.gitbook/assets/image (27).png>)

Note: Having a real controller connected wirelessly to the Switch, such as a Joy-Con, at the same time as JoyCon Droid can make the connection more stable in general for both amiibo and the connecting process (especially on games that disconnect controllers at start). You do not necessarily HAVE to use the Right JoyCon from the app, the Pro Controller from the app can work with this method too.

### Make sure to try changing your packet rate and testing other amiibos in JoyCon Droid Settings if this didn't work. <a href="#make-sure-to-also-lower-your-packet-rate-to-10-pps-in-joycon-droid-settings-if-this-didnt-work" id="make-sure-to-also-lower-your-packet-rate-to-10-pps-in-joycon-droid-settings-if-this-didnt-work"></a>

### Now you can try [using amiibos](using-amiibo.md)!
