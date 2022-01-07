# kernel

View Chinese description  |  [查看中文说明](README.cn.md)

Kernel repository that can be used to compile Armbian and OpenWer firmware.

## Description

- The kernel files stored in the [pub/stable](pub/stable) directory is a stable version produced and shared by [flippy](https://github.com/unifreq), suitable for use in a formal production environment.
- The kernel files stored in the [pub/dev](pub/dev) directory is a development version, and third-party driver support and special modifications have been added for some specific devices.
- The kernel files stored in the [pub/eol](pub/eol) directory are the kernel series that have stopped updating and are used for nostalgia.

The kernel files can be used in projects such as [amlogic-s9xxx-openwrt](https://github.com/ophub/amlogic-s9xxx-openwrt), [amlogic-s9xxx-armbian](https://github.com/ophub/amlogic-s9xxx-armbian), [flippy-openwrt-actions](https://github.com/ophub/flippy-openwrt-actions) and [unifreq/openwrt_packit](https://github.com/unifreq/openwrt_packit), etc. How to use it can be found in the description of each item.

## Compile a custom kernel

- For the compilation method of the custom kernel, see [compile-kernel](https://github.com/ophub/amlogic-s9xxx-armbian/tree/main/compile-kernel)


## Acknowledgments

- [flippy/kernel](https://github.com/unifreq)
- [armbian/build](https://github.com/armbian/build)
- [OpenWrt](https://github.com/openwrt/openwrt)
- [coolsnowwolf/lede](https://github.com/coolsnowwolf/lede)
- [Lienol/openwrt](https://github.com/Lienol/openwrt)

## License

[LICENSE](https://github.com/ophub/kernel/blob/main/LICENSE) © OPHUB

