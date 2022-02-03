# 内核

查看英文说明 | [View English description](README.md)

可用于编译 Armbian 和 OpenWer 固件的内核文件存储库。

## 说明

- 在 [pub/stable](pub/stable) 目录下存储的内核文件是 [flippy](https://github.com/unifreq) 制作分享的稳定版，适合在正式生产环境中使用。
- 在 [pub/dev](pub/dev) 目录下存储的内核文件是开发版，为一些特定盒子添加了第三方的驱动支持和特殊修改，供开发和测试使用。
- 在 [pub/eol](pub/eol) 目录下存储的内核文件是已经停止更新的内核系列，用于怀旧。

这些内核文件可以在 [amlogic-s9xxx-openwrt](https://github.com/ophub/amlogic-s9xxx-openwrt), [amlogic-s9xxx-armbian](https://github.com/ophub/amlogic-s9xxx-armbian), [flippy-openwrt-actions](https://github.com/ophub/flippy-openwrt-actions) 和 [unifreq/openwrt_packit](https://github.com/unifreq/openwrt_packit) 等项目中使用，具体使用方法可在各项目中查阅。

## 编译自定义内核

- 自定义内核的编译方法详见 [compile-kernel](https://github.com/ophub/amlogic-s9xxx-armbian/tree/main/compile-kernel), 使用 github.com 的 Actions 进行内核编译的模板可参考 [.yml](https://github.com/ophub/amlogic-s9xxx-openwrt/blob/main/.github/workflows/compile-kernel.yml)。

```yaml
- name: Compile the kernel for Amlogic s9xxx
  uses: ophub/amlogic-s9xxx-armbian@main
  with:
    build_target: kernel
    kernel_version: 5.15.13_5.4.170
    kernel_auto: true
    kernel_sign: -meson64-dev
```

## 鸣谢

- [flippy/kernel](https://github.com/unifreq)
- [armbian/build](https://github.com/armbian/build)
- [OpenWrt](https://github.com/openwrt/openwrt)
- [coolsnowwolf/lede](https://github.com/coolsnowwolf/lede)
- [Lienol/openwrt](https://github.com/Lienol/openwrt)

## License

[LICENSE](https://github.com/ophub/kernel/blob/main/LICENSE) © OPHUB

