# 第三方许可与对应源码 / Third-party notices and corresponding source

这些文件用于向二进制接收者提供已识别组件的必要许可、对应源码及构建资料。它们不是 Ketupa 核心源码，也不是产品安装包，不受第一方专有 EULA 覆盖。所有 Release 附件仍只放三个产品安装包。

These files provide required notices, corresponding source, and build materials for identified third-party binary components. They are neither proprietary Ketupa core source nor product installers, and retain their own licenses. Every Release still contains only three product installer attachments.

| 对应产品版本 / Product version | 组件 / Component | 源码 / Source | 原始来源 / Origin |
| --- | --- | --- | --- |
| 1.0.1 | 7-Zip 26.04 | [7z2604-src.tar.xz](sources/7z2604-src.tar.xz) | [Upstream / 上游](https://github.com/ip7z/7zip/releases/download/26.04/7z2604-src.tar.xz) |
| 1.0.1, Beta | CentOS GCC 4.8.5-44.el7 / libquadmath | [gcc-4.8.5-44.el7.src.rpm](sources/gcc-4.8.5-44.el7.src.rpm) | [Upstream / 上游](https://archive.kernel.org/centos-vault/7.9.2009/os/Source/SPackages/gcc-4.8.5-44.el7.src.rpm) |
| 1.0.1 | AlmaLinux GCC 8.5.0-26.el8_10.alma.1 / libquadmath | [gcc-8.5.0-26.el8_10.alma.1.src.rpm](sources/gcc-8.5.0-26.el8_10.alma.1.src.rpm) | [Upstream / 上游](https://vault.almalinux.org/8.10/BaseOS/Source/Packages/gcc-8.5.0-26.el8_10.alma.1.src.rpm) |
| Beta | FFmpeg 5.1.6 | [ffmpeg-5.1.6.tar.xz](sources/ffmpeg-5.1.6.tar.xz) | [Upstream / 上游](https://ffmpeg.org/releases/ffmpeg-5.1.6.tar.xz) |
| Beta | opencv-python-headless 4.11.0.86 build materials | [opencv-python-headless-4.11.0.86.tar.gz](sources/opencv-python-headless-4.11.0.86.tar.gz) | [Upstream / 上游](https://pypi.org/project/opencv-python-headless/4.11.0.86/) |

源码直接保存在本仓库。点击源码文件并使用 Download raw file 获取归档；GitHub 网页预览大小限制不影响原文件下载。GCC source RPM 包含对应发行版源码、补丁和构建 spec；不以通用新版替代对应版本。7-Zip 源码对应包内声明的未修改 26.04。Beta 的 FFmpeg 5.1.6 与 OpenCV Python 4.11.0.86 源分发对应已识别的共享库与构建材料；已检查的 FFmpeg 配置未启用 GPL/nonfree 开关。

Source archives are hosted directly in this repository. Use Download raw file to retrieve them; preview size limits do not prevent download. GCC source RPMs include matching distribution patches and build specs. The 7-Zip source matches the unmodified 26.04 build identified in the package notices. Beta's FFmpeg 5.1.6 and OpenCV Python 4.11.0.86 source distributions match identified shared-library and build materials; the inspected FFmpeg configuration did not enable GPL/nonfree flags.

历史两个 1.0.0 发行组的加密业务载荷未完全解码，不能据此声明完整依赖审计通过或“无需其他第三方材料”。安装包与源码归档内部版权、许可和组件声明应完整保留。如识别到其他缺失材料，请联系维护者补齐并审查受影响版本。原安装包字节保持不变；本次没有宣称真实安装、仿真验收或完整法律审计完成。

Encrypted business payloads in the two historical 1.0.0 distributions were not fully decoded. This does not establish a complete dependency audit or the absence of additional source obligations. Preserve all embedded notices, licenses, and component terms. Report missing materials to the maintainer for review of affected releases. Original installers remain byte-for-byte unchanged; this publication does not claim real installation, simulation acceptance, or a complete legal audit.

第一方 EULA 不撤销第三方许可明确保留的修改、替换和调试权利，也不授予绕过第一方专有软件授权的权利。完整组件声明以安装包与源码归档为准。

The first-party EULA does not revoke third-party rights to modify, replace, or debug components, and does not authorize bypassing proprietary Ketupa licensing. Consult the installers and source archives for complete component notices.

## 原许可 / Original licenses

- [7zip-LGPL-2.1.txt](licenses/7zip-LGPL-2.1.txt)
- [7zip-License.txt](licenses/7zip-License.txt)
- [7zip-unRAR-License.txt](licenses/7zip-unRAR-License.txt)
- [FFmpeg-LGPL-2.1.txt](licenses/FFmpeg-LGPL-2.1.txt)
- [OpenCV-Python-4.11.0.86-Third-Party.txt](licenses/OpenCV-Python-4.11.0.86-Third-Party.txt)
- [OpenCV-Python-Packaging-License.txt](licenses/OpenCV-Python-Packaging-License.txt)
- [SciPy-1.17.1-Third-Party.txt](licenses/SciPy-1.17.1-Third-Party.txt)

## SHA-256

```text
9691944c0fe0d01bb49373a704fb983fd33bc98b1738695179dfbf99ac1734f6  7z2604-src.tar.xz
642c4085f6af9565e39583e54a9d7a5d9e6b93dd8c8e9474aec8a892d6c7aa36  gcc-4.8.5-44.el7.src.rpm
0911864c260a75ae030f3144616e7e5e1359e04ce1c9730ab83906486e3bc79f  gcc-8.5.0-26.el8_10.alma.1.src.rpm
f4fa066278f7a47feab316fef905f4db0d5e9b589451949740f83972b30901bd  ffmpeg-5.1.6.tar.xz
996eb282ca4b43ec6a3972414de0e2331f5d9cda2b41091a49739c19fb843798  opencv-python-headless-4.11.0.86.tar.gz
```

Contact / 联系：[asenjoaupa@gmail.com](mailto:asenjoaupa@gmail.com)
