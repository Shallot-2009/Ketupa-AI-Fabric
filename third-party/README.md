# 第三方许可与对应源码 / Third-party notices and corresponding source

这些文件用于随 1.0.1 二进制分发提供必要的第三方许可和对应源码，不是 Ketupa 核心源码，不适用第一方专有 EULA。组件按各自原许可使用；完整声明以安装包和源码归档内文件为准。

These materials provide required third-party notices and corresponding source for the 1.0.1 binaries. They are not Ketupa core source code and are not governed by the first-party proprietary EULA. Each component retains its original terms; consult the installers and source archives for complete notices.

| 组件 / Component | 对应源码 / Source | 原始来源 / Origin |
| --- | --- | --- |
| 7-Zip 26.04 | [7z2604-src.tar.xz](sources/7z2604-src.tar.xz) | [Upstream / 上游](https://github.com/ip7z/7zip/releases/download/26.04/7z2604-src.tar.xz) |
| CentOS GCC 4.8.5-44.el7 / libquadmath | [gcc-4.8.5-44.el7.src.rpm](sources/gcc-4.8.5-44.el7.src.rpm) | [Upstream / 上游](https://archive.kernel.org/centos-vault/7.9.2009/os/Source/SPackages/gcc-4.8.5-44.el7.src.rpm) |
| AlmaLinux GCC 8.5.0-26.el8_10.alma.1 / libquadmath | [gcc-8.5.0-26.el8_10.alma.1.src.rpm](sources/gcc-8.5.0-26.el8_10.alma.1.src.rpm) | [Upstream / 上游](https://vault.almalinux.org/8.10/BaseOS/Source/Packages/gcc-8.5.0-26.el8_10.alma.1.src.rpm) |

源码直接存储在本仓库，点击文件后使用 Download raw file 获取原始归档；超过 GitHub 网页预览大小不影响下载。GCC 源码 RPM 包含对应发行版的补丁与构建资料；这不是只提供一个上游首页链接。7-Zip 源码为包内声明所对应的 26.04 原始版本。

Source archives are hosted directly in this repository. Use Download raw file to retrieve the original archive; GitHub preview size limits do not prevent downloading. GCC source RPMs contain matching distribution patches and build materials. The 7-Zip archive matches the unmodified 26.04 build identified in the package notices.

Selected original licenses / 部分原许可：

- [LGPL 2.1](licenses/7zip-LGPL-2.1.txt)
- [7-Zip](licenses/7zip-License.txt)
- [unRAR](licenses/7zip-unRAR-License.txt)
- [SciPy bundled components](licenses/SciPy-1.17.1-Third-Party.txt)

第一方 EULA 不撤销第三方许可授予的修改、替换和调试权利。原安装包保持字节不变。本页不宣称完整法律审计、安装测试或工程签核完成。历史版本已合法授予的权利不受本次下载页精简影响。

The first-party EULA does not revoke third-party rights to modify, replace, or debug components. Original installers remain byte-for-byte unchanged. This page does not claim a complete legal audit, installation testing, or engineering signoff. Streamlining the download page does not revoke rights lawfully granted for previous versions.

## SHA-256

```text
9691944c0fe0d01bb49373a704fb983fd33bc98b1738695179dfbf99ac1734f6  7z2604-src.tar.xz
642c4085f6af9565e39583e54a9d7a5d9e6b93dd8c8e9474aec8a892d6c7aa36  gcc-4.8.5-44.el7.src.rpm
0911864c260a75ae030f3144616e7e5e1359e04ce1c9730ab83906486e3bc79f  gcc-8.5.0-26.el8_10.alma.1.src.rpm
```

Contact / 联系：[asenjoaupa@gmail.com](mailto:asenjoaupa@gmail.com)
