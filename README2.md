# zigbee2mqtt

[![GitLab Sync](https://img.shields.io/badge/gitlab_sync-zigbee2mqtt-blue?style=for-the-badge&logo=gitlab)](https://gitlab-internal.spirit-dev.net/github-mirror/helm-zigbee2mqtt) <!-- markdownlint-disable MD041 -->
[![GitHub Mirror](https://img.shields.io/badge/github_mirror-zigbee2mqtt-blue?style=for-the-badge&logo=github)](https://github.com/spirit-dev/helm-zigbee2mqtt)
[![App Status](https://argocd-internal.spirit-dev.net/api/badge?name=zigbee2mqtt-turingpi&revision=true&showAppName=true)](https://argocd-internal.spirit-dev.net/applications/zigbee2mqtt-turingpi)

<!--TOC-->

- [Installation process](#installation-process)
- [Resources](#resources)

<!--TOC-->

## Installation process

The installation is entirely managed by Argocd.

A `Makefile` is present here to ease the first and one-time deployment or in case of an issue.
The installation should be done in two steps:

```shell
#> make dry-run ENV=<ENV>
#> make install ENV=<ENV>
```

## Resources

- [zigbee2mqtt helm installation](https://www.zigbee2mqtt.io/guide/installation/08_kubernetes.html#helm)

> Debugging information

- [Accurate configuration for Sonoff Zigbee Dongle - E](https://github.com/Koenkk/zigbee2mqtt/issues/25646#issuecomment-2575099501)
- [ember vs ezsp usb driver](https://github.com/Koenkk/zigbee2mqtt/discussions/21462)
- [Z2M crash kb](https://www.zigbee2mqtt.io/guide/installation/20_zigbee2mqtt-fails-to-start_crashes-runtime.html)

> USB Device: Sonoff Zigbee Dongle - E
> Flash information
>
> > To work properly, the Sonoff Dongle must be flashed with a `coordinator` version
>
> > Currently flashed with: https://github.com/darkxst/silabs-firmware-builder/blob/main/firmware_builds/zbdonglee/ncp-uart-hw-v7.4.4.0-zbdonglee-115200.gbl

- [Frimware list](https://github.com/darkxst/silabs-firmware-builder/blob/main/firmware_builds/zbdonglee)
- [Firmware list 2 (deprecated)](https://github.com/itead/Sonoff_Zigbee_Dongle_Firmware/tree/master/Dongle-E/NCP_7.4.4)
- [Flash procedure 1](https://www.zigbee2mqtt.io/devices/ZBDongle-E.html)
- [Flash procedure 2](https://sonoff.tech/wp-content/uploads/2022/11/SONOFF-Zigbee-3.0-USB-dongle-plus-firmware-flashing-.pdf)

> Blog installation

- [Installation using ser2sock](https://nikdoof.com/posts/2021/zigbee2mqtt-on-kubernetes/)
