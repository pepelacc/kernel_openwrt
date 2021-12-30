# kernel / 内核

Kernel repository that can be used to compile Armbian and OpenWer firmware.

可用于编译 Armbian 和 OpenWer 固件的内核文件存储库。

## Description / 说明

- Among them, the kernel files stored in the [pub/stable](pub/stable) directory is a stable version produced and shared by [flippy](https://github.com/unifreq), suitable for use in a formal production environment. The kernel files stored in the [pub/dev](pub/dev) directory are the kernel series that have stopped updating and the dev and beta kernel files collected from multiple channels, which are only used for testing. The kernel files can be used in projects such as [amlogic-s9xxx-openwrt](https://github.com/ophub/amlogic-s9xxx-openwrt), [amlogic-s9xxx-armbian](https://github.com/ophub/amlogic-s9xxx-armbian), [flippy-openwrt-actions](https://github.com/ophub/flippy-openwrt-actions) and [unifreq/openwrt_packit](https://github.com/unifreq/openwrt_packit), etc. How to use it can be found in the description of each item.

- 其中 [pub/stable](pub/stable) 目录下存储的内核文件是 [flippy](https://github.com/unifreq) 制作分享的稳定版，适合在正式生产环境中使用。在 [pub/dev](pub/dev) 目录下存储的内核文件为已经停止更新的内核系列，以及多渠道收集的开发版和测试版等内核文件，仅用于测试。内核文件可以在 [amlogic-s9xxx-openwrt](https://github.com/ophub/amlogic-s9xxx-openwrt), [amlogic-s9xxx-armbian](https://github.com/ophub/amlogic-s9xxx-armbian), [flippy-openwrt-actions](https://github.com/ophub/flippy-openwrt-actions) 和 [unifreq/openwrt_packit](https://github.com/unifreq/openwrt_packit) 等项目中使用，具体使用方法可在各项目中查阅。

## Compile a custom kernel / 编译自定义内核

- For the compilation method of the custom kernel, see [compile-kernel](https://github.com/ophub/amlogic-s9xxx-armbian/tree/main/compile-kernel)

- 自定义内核的编译方法详见 [compile-kernel](https://github.com/ophub/amlogic-s9xxx-armbian/tree/main/compile-kernel)

## Acknowledgments / 鸣谢

- [flippy/kernel](https://github.com/unifreq)
- [armbian/build](https://github.com/armbian/build)
- [OpenWrt](https://github.com/openwrt/openwrt)
- [coolsnowwolf/lede](https://github.com/coolsnowwolf/lede)
- [Lienol/openwrt](https://github.com/Lienol/openwrt)

## License

[LICENSE](https://github.com/ophub/kernel/blob/main/LICENSE) © OPHUB

