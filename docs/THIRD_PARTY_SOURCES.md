# 第三方源码与构建材料 / Third-party source and build materials

## 中文

以下附件是已识别第三方组件的源码材料，保留原项目许可；不包含 Ketupa 专有核心源码。源码包在相应版本的 Releases Assets 中，与安装包分开列示。不要将第三方源码包当作产品安装程序。

| 产品版本 / Product | 组件 / Component | 源码资产 / Source asset | Bytes |
| --- | --- | --- | --- |
| 1.0.1 | 7-Zip 26.04 | [7z2604-src.tar.xz](https://github.com/Shallot-2009/Ketupa-AI-Fabric/releases/download/v1.0.1/7z2604-src.tar.xz) | 1,560,440 |
| 1.0.1 | CentOS GCC 4.8.5-44.el7 / libquadmath | [gcc-4.8.5-44.el7.src.rpm](https://github.com/Shallot-2009/Ketupa-AI-Fabric/releases/download/v1.0.1/gcc-4.8.5-44.el7.src.rpm) | 79,314,655 |
| 1.0.1 | AlmaLinux GCC 8.5.0-26.el8_10.alma.1 / libquadmath | [gcc-8.5.0-26.el8_10.alma.1.src.rpm](https://github.com/Shallot-2009/Ketupa-AI-Fabric/releases/download/v1.0.1/gcc-8.5.0-26.el8_10.alma.1.src.rpm) | 65,714,006 |
| Beta | CentOS GCC 4.8.5-44.el7 / libquadmath | [gcc-4.8.5-44.el7.src.rpm](https://github.com/Shallot-2009/Ketupa-AI-Fabric/releases/download/beta/gcc-4.8.5-44.el7.src.rpm) | 79,314,655 |
| Beta | FFmpeg 5.1.6 | [ffmpeg-5.1.6.tar.xz](https://github.com/Shallot-2009/Ketupa-AI-Fabric/releases/download/beta/ffmpeg-5.1.6.tar.xz) | 10,021,428 |
| Beta | opencv-python-headless 4.11.0.86 build materials | [opencv-python-headless-4.11.0.86.tar.gz](https://github.com/Shallot-2009/Ketupa-AI-Fabric/releases/download/beta/opencv-python-headless-4.11.0.86.tar.gz) | 95,177,929 |

每个版本提供 `third-party-sources.json` 和 `THIRD_PARTY_SHA256SUMS.txt`，记录来源、大小及 SHA-256；安装包校验仍使用独立的 `SHA256SUMS.txt`。

### 对应关系与替换

- 1.0.1 的 7-Zip 来源说明指向未修改的官方 26.04；相应源码按上游发布资产哈希核验。
- 1.0.1 与 Beta 中 `96973f99` 家族的 libquadmath 按原始库哈希、构建标识及发行包记录追溯到 CentOS GCC 4.8.5-44.el7。1.0.1 中 `828275a7` 家族的调试链接标识对应 AlmaLinux 8.5.0-26.el8_10.alma.1。附原发行版 source RPM，包含源码、发行版补丁和构建 spec，不把通用最新版当作对应源码。wheel 打包可能调整库名、SONAME 和 RPATH，源码包不声称是已完成的逐字节可复现构建。
- Beta 的 OpenCV 4.11.0.86 携带 FFmpeg 5.1.6 共享库；已检查的配置未启用 GPL 或 nonfree 开关。附 FFmpeg 官方源码和匹配的 OpenCV Python 源分发，后者保留其构建脚本与第三方材料。各源码归档内部许可及组件条款优先，不能将全部组件统一改为 EULA。
- 对 LGPL 动态库的修改、替换，以及为调试这些修改而必要的逆向工程，按 LGPL 保留相应权利，不受第一方 EULA 的一般限制阻止。备份测试安装后，可使用 ABI 兼容的自建共享库替换相应第三方库；保留所需库名及加载路径。对 7-Zip 等独立工具可使用兼容的自建版本。此处不授权绕过 Ketupa 专有组件授权。
- 历史 1.0.0 的加密业务载荷未完全解码，本次不能推断其完整依赖组成；该版本的源码清单不表示“没有任何第三方依赖”。发现其他需要材料的组件，请联系维护者补齐并审查受影响发布。

版权、完整许可及通知随安装包和源码材料保留。联系：[asenjoaupa@gmail.com](mailto:asenjoaupa@gmail.com)。检查边界见 [发布核验范围](VERIFICATION.md)。

## English

These attachments provide source materials for identified third-party components under their original licenses. They do not contain the proprietary Ketupa core. Download them from the matching Release Assets; they are not product installers. Each release has `third-party-sources.json` and `THIRD_PARTY_SHA256SUMS.txt` for source provenance, sizes, and hashes. Installer hashes remain in the separate `SHA256SUMS.txt`.

- The 1.0.1 provenance notice identifies unmodified official 7-Zip 26.04. Its source is verified against the upstream release asset hash.
- The `96973f99` libquadmath family in 1.0.1 and Beta is traced to CentOS GCC 4.8.5-44.el7 using original-library hashes, build identifiers, and distribution records. The `828275a7` family in 1.0.1 identifies AlmaLinux 8.5.0-26.el8_10.alma.1 through its debug-link identifier. Original distribution source RPMs include source, distribution patches, and build specs. A generic latest release is not substituted. Wheel packaging may alter filenames, SONAME, and RPATH; source provision does not claim completed bit-for-bit reproducibility.
- Beta's OpenCV 4.11.0.86 includes FFmpeg 5.1.6 shared libraries; inspected configuration does not enable GPL or nonfree options. Official FFmpeg source and the matching OpenCV Python source distribution provide source and build materials. Archive-specific component terms govern; the EULA does not relicense these components.
- LGPL rights to modify and replace dynamic libraries, and to reverse engineer as necessary to debug those modifications, are retained despite general first-party EULA restrictions. Back up a test installation and replace the relevant shared library with an ABI-compatible self-built version, retaining required library names and loading paths. Compatible self-built standalone tools such as 7-Zip may also be used. This grants no right to bypass proprietary Ketupa licensing.
- The historical 1.0.0 encrypted business payload is not fully decoded, so its complete dependency composition is not established. Its source inventory does not assert the absence of third-party dependencies. Contact the maintainer about additional required materials so affected releases can be reviewed.

Preserve copyrights, full licenses, and notices supplied with installers and source materials. Contact [asenjoaupa@gmail.com](mailto:asenjoaupa@gmail.com). See [verification scope](VERIFICATION.md) for inspection limits.
