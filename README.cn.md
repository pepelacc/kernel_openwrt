# 内核

查看英文说明 | [View English description](README.md)

可用于编译 Armbian 和 OpenWer 固件的内核文件存储库。

## 说明

- 在 [pub/stable](pub/stable) 目录下存储的内核文件是 [unifreq](https://github.com/unifreq) 制作分享的稳定版，适合在正式生产环境中使用。
- 在 [pub/dev](pub/dev) 目录下存储的内核文件是开发版，为一些特定盒子添加了第三方的驱动支持和特殊修改，供开发和测试使用。
- 在 [pub/eol](pub/eol) 目录下存储的内核文件是已经停止更新的内核系列，用于怀旧。

这些内核文件可以在 [amlogic-s9xxx-openwrt](https://github.com/ophub/amlogic-s9xxx-openwrt), [amlogic-s9xxx-armbian](https://github.com/ophub/amlogic-s9xxx-armbian), [flippy-openwrt-actions](https://github.com/ophub/flippy-openwrt-actions) 和 [unifreq/openwrt_packit](https://github.com/unifreq/openwrt_packit) 等项目中使用，具体使用方法可在各项目中查阅。

## 编译自定义内核

- 自定义内核的编译方法详见 [compile-kernel](https://github.com/ophub/amlogic-s9xxx-armbian/tree/main/compile-kernel), 使用 github.com 的 Actions 进行内核编译的模板可参考 [.github/workflows/compile-kernel.yml](https://github.com/ophub/amlogic-s9xxx-openwrt/blob/main/.github/workflows/compile-kernel.yml)。
- 你可以根据需要对内核的配置进行调整，如添加驱动和补丁。也可以根据心情编译具有特殊意义的个性化签名内核，如 `5.10.95-happy-new-year`, `5.10.96-beijing-winter-olympics`, `5.10.99-valentines-day` 等等。

```yaml
- name: Compile the kernel for Amlogic s9xxx
  uses: ophub/amlogic-s9xxx-armbian@main
  with:
    build_target: kernel
    kernel_version: 5.10.100_5.4.180
    kernel_auto: true
    kernel_sign: -good-luck
```

## 鸣谢

- [unifreq/kernel](https://github.com/unifreq)
- [kernel.org](https://kernel.org)

## License

The kernel © OPHUB is licensed under [GPL-2.0](https://github.com/ophub/kernel/blob/main/LICENSE)
