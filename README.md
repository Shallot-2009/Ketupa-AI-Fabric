# Ketupa AI Fabric

[简体中文](#简体中文) | [English](#english)

**Ketupa AI 自动化设计与仿真 · 产品发布与下载**  
**Ketupa AI automated design and simulation · Product releases and downloads**

## 简体中文

本仓库是 Ketupa 产品安装包、版本说明和使用资料的发布专栏。核心为闭源专有软件，使用需要有效授权；公开下载不代表免费商用或取得源码许可。

### 下载与版本

| 版本 | 状态 | 安装包 | 下载 |
| --- | --- | --- | --- |
| 1.0.1 | 当前预览版；正式安装和真实仿真验收尚未完成 | Windows x64、Linux x64 TAR.GZ、Linux amd64 DEB，共 3 个 | [1.0.1](https://github.com/Shallot-2009/Ketupa-AI-Fabric/releases/tag/v1.0.1) |
| 1.0.0 | 历史稳定通道；保留原 runtime 与 openketupa 命名 | Windows、Linux 两套历史包，共 6 个 | [1.0.0](https://github.com/Shallot-2009/Ketupa-AI-Fabric/releases/tag/v1.0.0) |
| Beta | 历史测试版 | Windows x64、Linux x64 TAR.GZ、Linux amd64 DEB，共 3 个 | [Beta](https://github.com/Shallot-2009/Ketupa-AI-Fabric/releases/tag/beta) |

完整文件名、大小、SHA-256 和直接下载链接见 [下载清单](docs/DOWNLOADS.md) 与 [机器可读清单](catalog.json)。安装包在 GitHub Releases 的 Assets 中；GitHub 自动生成的 Source code ZIP/TAR 仅包含本仓库资料，不能用于安装产品。

### 使用步骤

1. 阅读 [许可协议](EULA.md)，按系统下载一个适用安装包；同一产品的 TAR.GZ 和 DEB 是不同分发形式，不必重复安装。
2. 使用对应版本的 `SHA256SUMS.txt` 核验下载文件，步骤见 [安装与授权](docs/INSTALLATION.md)。
3. 安装或解压后，按照产品提示配置环境并导入有效 `.lic`；授权问题请联系 [asenjoaupa@gmail.com](mailto:asenjoaupa@gmail.com)。不要把授权文件、机器标识或客户数据提交到公开 Issue。
4. 商业 EDA 软件及其许可证由使用者另外准备；本下载不授予 Ansys、Cadence、MATLAB 等软件的使用权。先在测试环境验收再投入业务。

### 许可与支持

- 本产品第一方专有组件适用 [LICENSE.txt](LICENSE.txt) 和 [EULA.md](EULA.md)，具体功能、设备数、期限与商业使用范围以有效授权或书面合同为准。
- 第三方组件保留各自权利，见 [第三方声明](THIRD_PARTY_NOTICES.md)。本仓库不撤销历史版本已经合法授予的权利。
- 本仓库不提供核心源码、授权签名私钥、客户工程或真实授权文件。完整性检查不等于功能、安全或仿真精度认证。
- 问题反馈见 [支持与反馈](SUPPORT.md)；维护流程见 [发布运维](docs/OPERATIONS.md)。
- 本轮检查内容及未覆盖事项见 [发布核验范围](docs/VERIFICATION.md)；第三方源码附件见 [源码说明](docs/THIRD_PARTY_SOURCES.md)。

发布者：**asen-tech.com**；维护联系：**Asenjo.HB.L**。主页：[Shallot-2009](https://github.com/Shallot-2009/)。

## English

This repository is the product distribution hub for Ketupa installers, release notes, and usage documentation. First-party core components are proprietary and require a valid license. Public download does not grant free commercial use or a source-code license.

### Downloads and versions

| Version | Status | Packages | Download |
| --- | --- | --- | --- |
| 1.0.1 | Current preview; formal installation and real simulation acceptance remain incomplete | Windows x64, Linux x64 TAR.GZ, Linux amd64 DEB; 3 files | [1.0.1](https://github.com/Shallot-2009/Ketupa-AI-Fabric/releases/tag/v1.0.1) |
| 1.0.0 | Historical stable channel; original runtime and openketupa filenames retained | Two historical Windows/Linux package sets; 6 files | [1.0.0](https://github.com/Shallot-2009/Ketupa-AI-Fabric/releases/tag/v1.0.0) |
| Beta | Historical test release | Windows x64, Linux x64 TAR.GZ, Linux amd64 DEB; 3 files | [Beta](https://github.com/Shallot-2009/Ketupa-AI-Fabric/releases/tag/beta) |

See the [download index](docs/DOWNLOADS.md) and [machine-readable catalog](catalog.json) for exact filenames, sizes, SHA-256 hashes, and direct links. Installers are Release Assets. GitHub-generated Source code ZIP/TAR files contain only this repository's documentation and cannot install the product.

### Getting started

1. Read the [EULA](EULA.md) and download one suitable package. TAR.GZ and DEB are alternative distribution formats for the same product; installing both is unnecessary.
2. Verify the file against that release's `SHA256SUMS.txt`; see [installation and licensing](docs/INSTALLATION.md).
3. Install or extract the package, follow its environment configuration prompts, and import a valid `.lic` as instructed by the product. Contact [asenjoaupa@gmail.com](mailto:asenjoaupa@gmail.com) for licensing. Never post licenses, machine identifiers, or customer data in public Issues.
4. Commercial EDA software and its licenses must be obtained separately. These downloads do not grant rights to Ansys, Cadence, MATLAB, or other third-party products. Validate in a test environment before business use.

### Licensing and support

- First-party proprietary components are subject to [LICENSE.txt](LICENSE.txt) and [EULA.md](EULA.md). Features, device counts, duration, and commercial-use rights follow the valid entitlement or written agreement.
- Third-party rights are retained; see [third-party notices](THIRD_PARTY_NOTICES.md). This repository does not revoke rights lawfully granted for historical releases.
- Core source code, license-signing private keys, customer projects, and real license files are not distributed through the repository tree. Integrity checks are not functional, security, or simulation-accuracy certification.
- See [support](SUPPORT.md) for reporting issues and [release operations](docs/OPERATIONS.md) for maintenance.
- See [publication verification scope](docs/VERIFICATION.md) for checks and limitations, and [third-party sources](docs/THIRD_PARTY_SOURCES.md) for source attachments.

Publisher: **asen-tech.com**. Maintainer contact: **Asenjo.HB.L**. Profile: [Shallot-2009](https://github.com/Shallot-2009/).
