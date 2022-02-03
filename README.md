# kernel

View Chinese description  |  [查看中文说明](README.cn.md)

Kernel repository that can be used to compile Armbian and OpenWer firmware.

## Description

- The kernel files stored in the [pub/stable](pub/stable) directory is a stable version produced and shared by [flippy](https://github.com/unifreq), suitable for use in a formal production environment.
- The kernel files stored in the [pub/dev](pub/dev) directory is a development version, and third-party driver support and special modifications have been added for some specific devices, for development and testing use.
- The kernel files stored in the [pub/eol](pub/eol) directory are the kernel series that have stopped updating and are used for nostalgia.

The kernel files can be used in projects such as [amlogic-s9xxx-openwrt](https://github.com/ophub/amlogic-s9xxx-openwrt), [amlogic-s9xxx-armbian](https://github.com/ophub/amlogic-s9xxx-armbian), [flippy-openwrt-actions](https://github.com/ophub/flippy-openwrt-actions) and [unifreq/openwrt_packit](https://github.com/unifreq/openwrt_packit), etc. How to use it can be found in the description of each item.

## Compile a custom kernel

- For the compilation method of the custom kernel, see [compile-kernel](https://github.com/ophub/amlogic-s9xxx-armbian/tree/main/compile-kernel), The template for kernel compilation using github.com's Actions can be found in [.yml](https://github.com/ophub/amlogic-s9xxx-openwrt/blob/main/.github/workflows/compile-kernel.yml).

```yaml
- name: Compile the kernel for Amlogic s9xxx
  uses: ophub/amlogic-s9xxx-armbian@main
  with:
    build_target: kernel
    kernel_version: 5.15.13_5.4.170
    kernel_auto: true
    kernel_sign: -meson64-dev
```

## Acknowledgments

- [flippy/kernel](https://github.com/unifreq)
- [armbian/build](https://github.com/armbian/build)
- [OpenWrt](https://github.com/openwrt/openwrt)
- [coolsnowwolf/lede](https://github.com/coolsnowwolf/lede)
- [Lienol/openwrt](https://github.com/Lienol/openwrt)

## License

[LICENSE](https://github.com/ophub/kernel/blob/main/LICENSE) © OPHUB

