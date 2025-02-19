# BetaFPV Beta75X 2S 穿越机

<Badge type="error" text="Discontinued" />

:::warning
This frame has been [discontinued](../flight_controller/autopilot_experimental.md) and is no longer commercially available.
:::

The [BetaFPV Beta75X](https://betafpv.com/products/beta75x-2s-whoop-quadcopter) is a very small quadrotor that can be flown indoors or outdoors, FPV or line-of-sight.

![BetaFPV Beta75X](../../assets/hardware/betafpv_beta75x.jpg)

## 购买渠道

另外你还需要一些其它的配件：

- [GetFPV](https://www.getfpv.com/beta75x-2s-brushless-whoop-micro-quadcopter-xt30-frsky.html)
- [Amazon](https://www.amazon.com/BETAFPV-Beta75X-Brushless-Quadcopter-Smartaudio/dp/B07H86XSPW)

In addition you will need:

- 一个遥控器以及接收机。 _Beta75X_ can ship with a number of receivers. PX4 能够兼容这些版本的接收机, 但请务必选择与您的遥控器 匹配的版本。
- 锂电池充电器 (飞机发货时包含一块电池, 但你可能想要额外备用的)。
- FPV goggles if you want to fly FPV. There are many compatible options, including these ones from [Fatshark](https://www.fatshark.com/product-page/dominator-v3).

  :::note
FPV support is completely independent of PX4/flight controller.
:::

## 刷写 Bootloader

The _Beta75X_ comes preinstalled with Betaflight.

Before loading PX4 firmware you must first install the PX4 bootloader. Instructions for installing the bootloader can be found in the [Omnibus F4](../flight_controller/omnibus_f4_sd.md#bootloader) topic (this is the flight controller board on the _Beta75X_).

:::tip
You can always [reinstall Betaflight](../advanced_config/bootloader_update_from_betaflight.md#reinstall-betaflight) later if you want!
:::

## 安装配置

Once the bootloader is installed, you should be able to connect the vehicle to _QGroundControl_ via a USB cable.

:::note
At time of writing _Omnibus F4_ is supported on the QGroundControl _Daily Build_, and prebuilt firmware is provided for the master branch only (stable releases are not yet available).
:::

To install and configure PX4:

- [首先更新PX4 固件目录](../config/firmware.md)。
- [Set the Airframe](../config/airframe.md) to _BetaFPV Beta75X 2S Brushless Whoop_.
- 再继续进行一些[基本配置](../config/README.md)，包括传感器校准和电台设置。

## 视频

@[youtube](https://youtu.be/_-O0kv0Qsh4)
