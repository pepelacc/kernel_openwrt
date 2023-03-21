# Kernel Description

View Chinese description  |  [查看中文说明](README.cn.md)

Kernel repository that can be used to compile Armbian and OpenWrt system. Kernel files with the `flippy` flag in their names are files made by [unifreq](https://github.com/unifreq), The files named by other names are the files I compiled using his kernel source code.

- The kernel files stored in the [pub/stable](pub/stable) directory is a `stable version`, suitable for use in a formal production environment.
- The kernel files stored in the [pub/rk3588](pub/rk3588) directory is a `special version` of the rk3588 series, which is suitable for devices such as Rock-5B and HinLink-H88K, and is not common to other series.
- The kernel files stored in the [pub/h6](pub/h6) directory is a `special version` made by [13584452567](https://github.com/13584452567/linux-6.1.y) for the Allwinner H6 series, which is suitable for devices such as TQC-A01, and is not common to other series.
- The kernel files stored in the [pub/dev](pub/dev) directory is a `development version`, and third-party driver support and special modifications have been added for some specific devices, for development and testing use.
- In [dev](https://github.com/ophub/kernel/releases/tag/dev) of Releases, there is a download image of the `cross-compilation toolchain` required for compiling the kernel.
- In the [tools](https://github.com/ophub/kernel/releases/tag/tools) of Releases, there are some `Android system` download images of common TV boxes. When using Armbian and OpenWrt systems, you can use It is used to restore the Android system.

## Use the kernel

This kernel can be used in `Armbian` and `OpenWrt` systems. For example [amlogic-s9xxx-armbian](https://github.com/ophub/amlogic-s9xxx-armbian), [amlogic-s9xxx-openwrt](https://github.com/ophub/amlogic-s9xxx-openwrt), [flippy-openwrt-actions](https://github.com/ophub/flippy-openwrt-actions) and [unifreq/openwrt_packit](https://github.com/unifreq/openwrt_packit). It can be integrated when compiling firmware, or it can be installed into an existing system for use. For specific usage, please refer to [Kernel usage Instructions](https://github.com/ophub/amlogic-s9xxx-armbian/blob/main/compile-kernel/README.md#kernel-usage-instructions).

## Compile the kernel

- You can adjust the configuration of the kernel as needed, such as adding drivers and patches. It is also possible to compile personalized signature kernels with special meanings according to mood, such as `5.10.95-happy-new-year`, `5.10.96-beijing-winter-olympics`, `5.10.99-valentines-day` and so on.

- For the compilation method of the kernel, see [compile-kernel](https://github.com/ophub/amlogic-s9xxx-armbian/tree/main/compile-kernel), The template for kernel compilation using github.com's Actions can be found in [.github/workflows/compile-kernel.yml](https://github.com/ophub/amlogic-s9xxx-openwrt/blob/main/.github/workflows/compile-kernel.yml).

```yaml
- name: Compile the kernel
  uses: ophub/amlogic-s9xxx-armbian@main
  with:
    build_target: kernel
    kernel_version: 5.10.135_5.15.50
    kernel_auto: true
    kernel_sign: -yourname
```

## Links

- [unifreq/kernel](https://github.com/unifreq)
- [13584452567/kernel](https://github.com/13584452567/linux-6.1.y)
- [chewitt/linux](https://github.com/chewitt/linux)
- [torvalds/linux](https://github.com/torvalds/linux)
- [kernel.org](https://kernel.org)

## License

The kernel © OPHUB is licensed under [GPL-2.0](https://github.com/ophub/kernel/blob/main/LICENSE)
