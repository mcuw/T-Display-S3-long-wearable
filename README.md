# ESP32 - LilyGo T-Display S3 long weareable

## Description

This is a project about the wearable 4 you in 2024.
Interactions with a great smart capacity touch display.

## Requirements

LILYGO board: https://www.lilygo.cc/products/t-display-s3-long

Buy and support mcuw on aliexpress (affiliate link): https://s.click.aliexpress.com/e/_DEv67TX

## Board Specification

- AXS15231 In-Cell IC Integrates 540-channel Source Driver and GIP Gate Driver and Touch Panel Controller Into a Single Chip with TP Controller Supports Real Multi-Touch Capability

## Power consumption

| Mode                          | power consumption [Ah] | description                                                                                                                               |
| ----------------------------- | ---------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- |
| display                       | 0.13 - 0.14            | [example/TFT](https://github.com/Xinyuan-LilyGO/T-Display-S3-Long/tree/ee16b751263df00454a3ccef5414c82307ea04a7/examples/TFT)             |
| display + wifi                | 0.14 - 0.16            | [example/factory](https://github.com/Xinyuan-LilyGO/T-Display-S3-Long/tree/ee16b751263df00454a3ccef5414c82307ea04a7/examples/factory)     |
| display + touch               | 0.13 - 0.17            | [example/lvgl_demo](https://github.com/Xinyuan-LilyGO/T-Display-S3-Long/tree/ee16b751263df00454a3ccef5414c82307ea04a7/examples/lvgl_demo) |
| touch + serial + black screen | 0.05 - 0.07            | [examples/touch](https://github.com/Xinyuan-LilyGO/T-Display-S3-Long/tree/ee16b751263df00454a3ccef5414c82307ea04a7/examples/touch)        |

possibilies to reduce power consumptions:

- lower brightness (min. ~100 as value)
- reduce CPU freq (min. 80MHz for Wifi/ BT)
- Deepsleep with touch on (uA) or Light Sleep (continues afterwards w/o reset)
- zero power - with Mosfet and hold on after click push button
- own optimized board design

## Disclaimer

Contribution and help ... if you find an issue or wants to contribute then please do not hesitate to create a merge request or an issue.

We provide our build template as is, and we make no promises or guarantees about this code.
